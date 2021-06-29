# milestoneI

Abstract

Crude oil is the largest global energy source. Its refined products are vital inputs to nearly all modern economies and its industrial applications can be seen in major industries throughout the world. This function has made crude oil one of the most important commodities of the last century. It is traded in global markets and many financial institutions are heavily invested in its performance. Some market commentators even draw parallels between the price of crude oil and the behavior of financial markets. This study seeks to analyze the validity of these claims by observing the correlation between petroleum product spot prices and business sector performance over the last 15 years.
Introduction
Crude oil is a fossil fuel composed of hydrocarbons that formed from the remains of plants and animals that lived millions of years ago. This fuel is a non-renewable resource that exists in liquid form inside underground reservoirs. After being removed from the ground, crude oil mixtures can be refined and separated into useful petroleum products including gasoline, diesel fuel, heating oil, jet fuel, petrochemical feedstocks, waxes, lubricants, asphalt, and other extracts (EIA, 2021).
     

After these industrial uses were discovered in the 19th century, crude oil production increased rapidly to fuel the transition from agrarian to manufacturing societies. This industrialization ultimately enabled the creation of a modern global economy, and while investment in renewable energies such as solar and wind power has increased significantly in recent years, crude oil is still the world’s primary source of energy production (Chen, 2021).
This role in energy production makes crude oil vital to the global economic framework and a foundational resource for many of the largest global industries:


Motivation

Given this importance in modern economic activities, crude oil is traded in commodity markets throughout the world and many financial institutions have developed mechanisms for investors to gain exposure to the oil industry through instruments such as oil futures, options, exchange-traded funds, and mutual funds (Chen, 2021).
This entanglement with financial markets has led many speculators to question the impact of oil prices on financial markets. However, while market commentators often use these instruments to draw parallels between changes in oil prices and market behavior on specific days, many communities are unsure of the relationship between the price of petroleum products and the performance of financial markets in the long term (The Associated Press, 2021; Pescatori, 2021). One study performed by the Federal Reserve Bank of Cleveland even suggests that there is no significant correlation between oil prices and the stock market (Pescatori, 2021).
This study seeks to enter this area of research by analyzing claims of correlation between the price of petroleum products and the performance of various financial markets and sectors. 

Specifically, the goal of this analysis is to answer:

What is the relationship between oil product prices on U.S. financial markets?

What is the relationship between oil product prices on different U.S. business sectors?

Researching these topics will guide this study as it investigates whether petroleum product prices are correlated with the value of various instruments and whether crude oil prices are a meaningful input in financial models built to forecast the performance of financial securities.

Data Sources

Crude Oil Product Spot Prices

To answer the goals stated above, two data sources will be required.. The first data source is published by the United States Energy Information Administration (EIA) and stores historical spot prices on crude oil and its derivatives.

Crude Oil & Petroleum Spot Prices

Contains historical daily spot prices on Crude Oil and some of its derivatives: Conventional Gasoline, RBOB Regular Gasoline, Heating Oil, Diesel Fuel, Kerosene Jet Fuel, and Propane.

Located at: https://www.eia.gov/dnav/pet/pet_pri_spt_s1_d.htm

XLS file: https://www.eia.gov/dnav/pet/xls/PET_PRI_SPT_S1_D.xls 

Downloading the entire series of data made available will return a .XLS file containing crude oil, conventional gasoline, regular gasoline, heating oil, diesel, jet fuel, and propane historical prices. The daily spot prices go back as far as 1986 for certain gas products and the entire file is 3.1 MB. Although not used in this analysis, the EIA API can be used to access this data directly. Documentation for the API can be found here.

Financial Market Data

The second dataset is published by IEX Group. IEX Cloud is an API that allows developers to access a wide array of curated financial data. The platform returns JSON-encoded responses on specific financial securities based on requests sent to the API. An API key is required to call the API. When registering for a key, you have the option for free access or a more robust paid version.

The API can be requested at: https://cloud.iexapis.com/stable

The data catalog can be found at: https://iexcloud.io/core-data-catalog

Register for an API key: https://iexcloud.io/cloud-login#/register

This study uses the IEX Cloud API to obtain historical price data on business sectors and individual securities. The API is called twelve times to represent each business sector and the overall market. From the API response, data from the past 15 years from March 31, 2021 will be needed, or 3544 entries each. 

Energy -  Energy Select Sector SPDR Fund (XLE) 

Materials - Materials Select Sector SPDR Fund (XLB) 

Consumer Discretionary - Consumer Discretionary Select Sector SPDR Fund (XLY)

Consumer Staples - Consumer Staples Select Sector SPDR Fund (XLP)

Industrials - Industrial Select Sector SPDR Fund (XLI) 

Utilities - Utilities Select Sector SPDR Fund (XLU) 

Healthcare - Health Care Select Sector SPDR Fund (XLV) 

Financials - Financial Select Sector SPDR Fund (XLF) 

Information Technology - iShares Expanded Tech Sector ETF (IGM)

Communication Services - iShares Global Comm Services ETF (IXP)

Real Estate - Shares US Real Estate ETF (IYR)

S&P 500 - SPDR S&P 500 ETF Trust (SPY)

To control the effects of individual securities and to limit the size of the dataset, this study will be analyzing sector performance using the closing price data on business sector exchange traded funds (ETFs).

Conclusions

The time series and heatmap correlation analysis indicate valuable trends in the relationship between WTI spot prices and business sector ETF prices. The major observations from this analysis include:

Market value increases in the long-term, while oil prices are relatively stagnant.

Oil prices are significantly more volatile than each business sector.

Oil prices are generally negatively correlated with business sector performance in the long-term.

Business sector performance and oil prices appear to be positively correlated in the short term in specific situations (recessions, recoveries), but this trend does not hold over long periods of time.

The energy sector is the only business sector with a positive correlation to oil prices. This is also the strongest correlation between oil prices and any business sector.

The global communication services sector has the weakest correlation with oil prices. 

The heatmap suggests there is moderate correlation between the overall financial market and oil prices.

While these observations can be made, one must remember that correlation does not mean causation. Correlation indicates how strongly two variables are linearly related and change together (Singh, 2019). Causation indicates any change in the value of one variable will cause a change in the value of another variable. One should not take the analysis conducted in this report to make claims about the price of oil and the short-term performance of any business sector. Professional services should be sought for anyone seeking advice on personal investing decisions.

Although this study scratched the surface on the relationship between oil prices and business sector performance, further analysis must be taken to better understand the relationship between oil prices and financial markets. Some avenues for future research identified include:

Observing price shocks due to major recessionary events and recovery periods.

Observing price shocks due to decisions made by the Organization of Petroleum Exporting Countries.

Observing oil prices and business sector performance at specific points in time using a sentiment analysis of major news headlines.

Better understanding the relationship between oil prices and specific business sectors by observing each individual sub-sectors in each ETF analyzed.

References

Beitsch, Rebecca. “Oil Trades at Lowest Price in History after Slipping into Negative Pricing.” TheHill, The Hill, 20 Apr. 2020, https://thehill.com/policy/energy-environment/493688-oil-trades-below-8-a-barrel-hitting-30-year-low#:~:text=Oil%20hit%20%240.01%20a%20barrel,trading%20oil%20futures%20in%201983.

Chen, James. “Crude Oil.” Investopedia, Investopedia, 19 May 2021, www.investopedia.com/terms/c/crude-oil.asp.

Fernando, Jason. “Correlation Coefficient Definition.” Investopedia, Investopedia, 19 May 2021, www.investopedia.com/terms/c/correlationcoefficient.asp.

“Gas Prices Decrease for First Time This Year.” Tullahoma News, 1 Apr. 2021, www.tullahomanews.com/news/local/gas-prices-decrease-for-first-time-this-year/article_51603dbc-931f-11eb-8572-67ec48eff572.html.

Green, Matthew et al. “Past Its Peak? Battered Oil Demand Faces Threat from Electric Vehicles.” Reuters, Thomson Reuters, 19 May 2020, www.reuters.com/article/us-data-esg-autos/past-its-peak-battered-oil-demand-faces-threat-from-electric-vehicles-idUSKBN22V1HY.

Hecht, Andrew. “The Price of Crude Oil and Equity Prices.” The Balance, www.thebalance.com/the-price-of-crude-oil-and-equity-prices-808866.

“Industry Market Research, Reports, and Statistics.” IBISWorld, www.ibisworld.com/global/industry-trends/biggest-industries-by-revenue/.

The Associated Press. “UPDATE: Wall Street Rebounds as the Price of Oil Falls Back.” Ajc, The Atlanta Journal-Constitution, 25 Mar. 2021, www.ajc.com/news/nation-world/stocks-slip-on-wall-street-as-the-price-of-oil-falls-back/3U6A6ZQNC5HJZDZPTBIJPYT6LE/.

Patel, Nihar. “Effect of Rising Oil Prices on the Stock Market.” Finance, 7 Feb. 2017, finance.zacks.com/effect-rising-oil-prices-stock-market-5479.html.

Pescatori, Andrea. “Do Oil Prices Directly Affect the Stock Market?” Website, Federal Reserve Bank of Cleveland, 12 Sept. 2008, www.clevelandfed.org/newsroom-and-events/publications/economic-trends/economic-trends-archives/2008-economic-trends/et-20080912-do-oil-prices-directly-affect-the-stock-market.aspx.

Singh, Seema. “Why Correlation Does Not Imply Causation?” Medium, Towards Data Science, 2 Jan. 2019, https://towardsdatascience.com/why-correlation-does-not-imply-causation-5b99790df07e.

Tobben, Sheela. “Negative Oil Prices: What Does Oil Below Zero Really Mean?” Bloomberg.com, Bloomberg, 20 Apr. 2020, www.bloomberg.com/news/articles/2020-04-20/negative-prices-for-oil-here-s-what-that-means-quicktake.

“U.S. Energy Information Administration - EIA - Independent Statistics and Analysis.” Oil and Petroleum Products Explained - U.S. Energy Information Administration (EIA), www.eia.gov/energyexplained/oil-and-petroleum-products/.

“U.S. Energy Information Administration - EIA - Independent Statistics and Analysis.” Refining Crude Oil - Inputs and Outputs - U.S. Energy Information Administration (EIA), www.eia.gov/energyexplained/oil-and-petroleum-products/refining-crude-oil-inputs-and-outputs.php.

“XLE: The Energy Select Sector SPDR® Fund.” State Street Global Advisors, www.ssga.com/us/en/institutional/etfs/funds/the-energy-select-sector-spdr-fund-xle.
