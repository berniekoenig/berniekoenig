- 👋 Hi, I’m @berniekoenig

I'm trying to learn how to manipulate python pandas DataFrames.  Here is some sample code :

import pandas as pd
Income_Data=pd.read_csv(\'C:\Users\Bkoenig\InvestingMachineLearning/us-income-annual.csv',\delimiter=";")

This is what I'm doing and I keep getting the following error:

File "<ipython-input-1-a1dd9d02779d>", line 2
    Income_Data = pd.read_csv(\'C:\Users\Bkoenig\InvestingMachineLearning/us-income-annual.csv', \ delimiter=";")
                                                                                                                ^
SyntaxError: unexpected character after line continuation character

I tried taking out the backslashes and I got this error:

SyntaxError: (unicode error) 'unicodeescape' codec can't decode bytes in position 2-3: truncated \UXXXXXXXX escape

How can I load a *.csv file, use it as a DataFrame, and access say the highest 'Net Income" in the file (['Net Income'].max) and the corresponding Ticker symbol?

Any help would be greatly appreciated :)

Below is a sample of what the *.csv looks like:

Ticker;SimFinId;Currency;"Fiscal Year";"Fiscal Period";"Report Date";"Publish Date";"Restated Date";"Shares (Basic)";"Shares (Diluted)";Revenue;"Cost of Revenue";"Gross Profit";"Operating Expenses";"Selling, General & Administrative";"Research & Development";"Depreciation & Amortization";"Operating Income (Loss)";"Non-Operating Income (Loss)";"Interest Expense, Net";"Pretax Income (Loss), Adj.";"Abnormal Gains (Losses)";"Pretax Income (Loss)";"Income Tax (Expense) Benefit, Net";"Income (Loss) from Continuing Operations";"Net Extraordinary Gains (Losses)";"Net Income";"Net Income (Common)"
A;45846;USD;2016;FY;2016-10-31;2016-12-20;2018-12-20;326000000;329000000;4202000000;-2005000000;2197000000;-1582000000;-1253000000;-329000000;;615000000;-71000000;-61000000;544000000;;544000000;-82000000;462000000;;462000000;462000000
A;45846;USD;2017;FY;2017-10-31;2017-12-21;2018-12-20;322000000;326000000;4472000000;-2063000000;2409000000;-1568000000;-1229000000;-339000000;;841000000;-38000000;-57000000;803000000;;803000000;-119000000;684000000;;684000000;684000000
A;45846;USD;2018;FY;2018-10-31;2018-12-20;2020-12-18;321000000;325000000;4914000000;-2234000000;2680000000;-1776000000;-1389000000;-387000000;;904000000;42000000;-37000000;946000000;;946000000;-630000000;316000000;;316000000;316000000
A;45846;USD;2019;FY;2019-10-31;2019-12-19;2021-12-17;314000000;318000000;5163000000;-2358000000;2805000000;-1864000000;-1460000000;-404000000;;941000000;-22000000;-38000000;919000000;;919000000;152000000;1071000000;;1071000000;1071000000
A;45846;USD;2020;FY;2020-10-31;2020-12-18;2021-12-
