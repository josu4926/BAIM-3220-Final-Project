# BAIM-3220-Final-Project

**Introduction**

For our final project we will be creating an .ipynb notebook that works in conjunction with the Yahoo Finance API. The goal of our project was to scrape data online, filter and manipulate the data, and form analysis on the data which we created. 

**Process**

We began the project by working on implementing the Yahoo Finance API into the .ipynb notebook. Following this, we selected the five stocks and set the time window of 30 years which we were going to create our project around. Next, we began by filtering the Yahoo Finance data. Each of the stock tickers contained variables such as “high”, “low”, “opening”, “close”, “adjclose”, and “volume”. Then, we limited the data to just “open” and “close” data. From there, we created two new variables which determined the percentage change of the “open” to “close” values and then a variable which calculated the average of the percentage changes over the 30 years.

Now that all of our data was compiled we began running a KNN data creation script to give us dates to look at where each of the five stocks had similar percentage change values. Following this, we began running regression models for each of the stocks to create lines of best fits to see how each of the stocks would perform based on the rest of the group. The variables we were comparing were the percentage change on the stock for each day. 

**Analysis**

Before we begin our analysis it is important to understand how we chose our dates.

KNN: We took the closing percentage changes for the 5 stocks on May 2nd 2023 in order to determine what historical data was closest to these current changes. All changes for that date that we used were negative, therefore when it came to the KNN it was normally times of distress for the company. As we can see from the data presented in the KNN graph, Apple, TSMC and  Microsoft have consistently experienced these negative changes in stock price from 2005-2018. When it came to the other 2 stocks, NVIDIA and Intel, the volatility of changes were more extreme and therefore the graph shows the points bouncing all over the place from 2005-2018.

These are the dates that we are building our analysis off of for each stock ticker 

September 24, 2004: US Commerce Department announced the US economy had grown at a faster-than-expected rate of 3.3% in the second quarter of 2004. This was a positive sign for the US economy and had a positive impact on the stock market. The Dow Jones closed up 43 points.
Stocks listed on the tech-focused Nasdaq were generally oversold far more this year due to a weaker technology sector

December 01, 2006: The US Labor Department announced that unemployment had fallen to the lowest level in more than five years: 4.5%. This was seen as a positive for the US economy as it had a positive impact on the stock market, evident as the Dow Jones closed up 61 points.
    Among tech stocks, chip shares tumbled. Chipmakers AMD (Charts) and Nvidia (Charts) both slid about 4 percent. The Department of Justice has subpoenaed both companies in relation to an investigation into antitrust violations.
    Intel (Charts), the world's largest maker of chips for PCs, said it didn't believe it was a target of the DoJ probe, but shares fell 3 percent after rival AMD said it was gearing up to offer a new chip next year.

March 07, 2007: The Dow Jones hit a record high on this day of 12,765. The market had been on a steady upward trend since 2003, mostly due to strong corporate earnings and low interest rates. The record high was seen as a positive sign for the economy and had a positive impact on the stock market. 

October 20, 2009: The Federal Reserve announced that it would keep interest rates near 0 for an extended period of time in order to stimulate economic growth.       This was a major positive for the economy and the stock market. The Dow Jones closed up 131 points.
    Thanks to an aggressive expansion into international markets, Apple now has 18% of the global market share in these high-end devices (behind Nokia and BlackBerry maker Research in Motion), up from 14% in the second quarter of 2009. And Apple is just getting started.

January 12, 2010: The Supreme Court issues its ruling in the Citizens United Case on this day which lifted restrictions on corporate and union spending in political campaigns. This news had a mixed impact on the stock market as it was positive for media and advertising industries, but negative for consumer groups. The Dow Jones closed down 37 points.

December 13, 2010: The Obama administration reached a compromise on this day with congressional Republicans on a tax package that extended the Bush-era tax cuts as well as other measures aimed to boost the economy. The Dow Jones closed up 55 points this day.
After electronics manufacturers -- enthusiastic about an economic recovery -- overbought global chip supplies in early 2010, demand slowed in recent months as they used up inventories.

August 23, 2012: The Federal Reserve announced a plan to launch a third round of quantitative easing known as QE3. This was perceived as a positive for the US economy as the goal of it was to boost economic growth and lower unemployment. The Dow Jones closed up 144 points following this announcement. 
After a three-week trial, a federal court jury presented a verdict in the lengthy patent infringement lawsuit between Samsung and Apple. Samsung was found to have knowingly infringed on Apple patents, with damages totaling more than $1 billion. On the other hand, the jury found Apple not guilty in all five instances cited by Samsung.

July 24, 2015: China’s stock market experienced a major sell-off this day with the Shanghai Composite Index dropping more than 8%. This had a negative impact on global markets and the US stock market specifically which saw the Dow Jones close down 163 points.
AT&T completed its acquisition of DirecTV for $49 billion on July 24, 2015. CSR was acquired by Qualcomm on August 14, 2015, and renamed as Qualcomm Technologies International.

August 10, 2016: The US Labor Department released its monthly jobs report which showed the economy had added more jobs than expected in July: 255,000. This was seen as a major positive for the stock market and the economy and the Dow Jones closed up 191 points. 

March 06, 2019: The European Central Bank (ECB) announced a new round of stimulus measures aimed at boosting the Eurozone economy. This news was seen as a positive sign for global economic growth and had a positive impact on the stock market. The Dow Jones closed up 148 points.

