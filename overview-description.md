# ApparelBankruptcyAnalysis
Title Apparel Industry Bankruptcy Analysis 

Objective: Identify apparel industry companies (publicly traded) that are at risk for bankruptcy. Did this by creating an industry scoring system to rank companies from an Excellent to Weak Financial Position. Any company with a Weak Financial position would be identified to be at risk for bankruptcy. 

Data Source: https://www.kaggle.com/cnic92/200-financial-indicators-of-us-stocks-20142018

Project Details: 

Analysis:
I analyzed all 10K Filings Data from 2014-2018 and isolated the retail apparel (clothing & shoes) industry tickers. 
After isoalting the retail apparel industry, I created 4 benchmarks with key KPI figures to be used to analyze company performance. 

These 4 Benchmarks are: 
1. Profitability - Net Profit Margin Ratio, Return on Equity, & Return on Assets
2. Liquidity - Current Ratio & Quick Ratio
3. Efficiency - Inventory Turnover & Asset Turnover 
4. Solvency - Debt to Equity Ratio & Debt to Assets Ratio

Once my benchmarks were created, I calculated the average for each KPI over the 5 year period and I calculated the average annual % change for each KPI over the same period.
I then calculated the average and annual % change (over 5 years) for the industry as a whole to compare to each indiviudal company.

Scoring System:
The Apparel Industry Scoring System was created by comparing each individual company's average Profitability, Liquidity, Efficiency, and Solvency KPI's with the industry averages. This scoring sytem itself was designed to assign 1 point for every individual company's KPI that was above the industry average and annual % change average. 
Company's could earn 6 points for Profitabilty and 4 points each for Liquidity, Efficiency, and Solvency. 
On average companies scored 8 points with a minimum of 3 points scored and a maximum of 16. 

For example: 
AEO (American Eagle Outfitters) had an average Net Profit Margin of .04 when the industry average was a .05, therefore they received 0 points for that KPI indicator when they could have earned 1 point. 
AEO had a net profit margin average annual % change of .375 when the industry net profit margin average annual % change -.031, therefore they received 1 point for that KPI indicator. 

Ranking: 
Financial Position was determined based on how many points were scored by each company. 
Weak Financial Position: 0 - 5 points
Good Financial Position: 6 - 7 points
Great Financial Position: 8 - 10 points 
Excellent Financial Position : 11+ Points. 

Bankruptcy Analysis: 
I analyzed the operations, marketing, and business strategies for each company in the Weak and Excellent Financial Position to determine the key performance differences. Isolating the weak and excellent companies was key for understanding why certain companies were at risk for bankruptcy while others were thriving.
Results are in the Jupyter Notebook.

Data Validity
I compared the Altman Z-Sore (an official bankruptcy indicator) to each company with my Apparel Industry Score to see if they correlate. I found that the Altman Z-Score was very Asset heavy and most retail companies that are very successful were actually avoiding having large amounts of Assets on the balance sheet. This gave false positives and negatives using the Altman Z-Score. 






