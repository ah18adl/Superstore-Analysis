[SuperstoreSalesReadME.rtf](https://github.com/user-attachments/files/34519856/SuperstoreSalesReadME.rtf)
{\rtf1\ansi\ansicpg1252\cocoartf2870
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\fswiss\fcharset0 Helvetica;}
{\colortbl;\red255\green255\blue255;}
{\*\expandedcolortbl;;}
\paperw11900\paperh16840\margl1440\margr1440\vieww11520\viewh8400\viewkind0
\pard\tx720\tx1440\tx2160\tx2880\tx3600\tx4320\tx5040\tx5760\tx6480\tx7200\tx7920\tx8640\pardirnatural\partightenfactor0

\f0\fs24 \cf0 # Superstore Sales Performance Analysis\
\
## Business problem\
A US retail superstore wants to know what is driving its growth, where it is\
losing money, and what it should change to improve profit.\
\
## Data and cleaning\
- Superstore dataset (Kaggle): 9,994 order lines, 5,009 orders, 793 customers,\
  2014\'962017, across 4 US regions and 3 categories (Furniture, Office Supplies,\
  Technology).\
- No missing values found.\
- Dropped Row ID (a row counter) and Country (only one value: United States).\
- After removing Row ID, 1 hidden duplicate row appeared and was removed.\
- Each row is a product line within an order, so orders were counted with\
  unique Order IDs rather than rows.\
\
## Key findings\
1. **Growth is healthy.** Sales grew 51% from 2014 to 2017 and margin rose from\
   10% to 13%. Growth came from more orders, while average order value fell.\
2. **Heavy discounts destroy profit.** Margin is 30% with no discount but -15%\
   at 21\'9640% off and -77% above 40% off. Lines discounted above 20% are about\
   14% of all lines, but lost about 135k, roughly half of total profit (286k).\
3. **Central underperforms on margin.** Central's average discount is 24% vs\
   11% in West, and its margin is 8% vs 15%, even though it sells more than South.\
4. **Tables are the biggest loss-maker** (-17.7k profit), but make a 19% margin\
   at full price. The losses come from discounting, not pricing.\
\
## Recommendations\
1. **Cap discounts at 20%.** Require approval for anything higher.\
   Impact: halving the losses above 20% would add around 65k profit.\
2. **Bring Central's discounting in line with West's**, and investigate why it\
   is higher (for example, sales targets based on revenue rather than profit).\
   Impact: reaching West's 15% margin on Central's ~501k sales would add up to\
   about 35k profit.\
3. **Stop discounting Tables**, starting with a trial in one region and\
   comparing results before rolling it out.\
   Impact: up to a ~57k swing from a 17.7k loss to a profit, though some sales\
   may be lost.\
\
Note: these findings show associations, not proven causes. Heavily discounted\
items may be slow-selling stock, so changes should be tested before full rollout.\
\
## Tools and links\
- Python (pandas, matplotlib) in Jupyter\
- Tableau Public\
- Dashboard: https://public.tableau.com/views/SuperstoreSalesPerformanceAnalysis_17940568921770/Overview\
- Notebook: https://github.com/ah18adl/Superstore-Analysis}
