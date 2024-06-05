# Customer_Demography_Sorting-Filtering

# Problem Statements:
- Use the Filter and Sort tools
- Use IF, IFS, COUNTIF, and SUMIF functions for data analysis
- Use the VLOOKUP and HLOOKUP reference functions

# Dataset used: [Download the file Customer_demographics_and_sales_Lab6.xlsx. Upload and open it using Excel for the web.](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%206%20-%20Filtering%20and%20Sorting%20Data%20using%20Functions%20for%20Data%20Analysis/Customer_demographics_and_sales_Lab6.xlsx)

# Filtering and Sorting Data
  ### TaskA : Filtering Data
    - Select any cell in the data, and click the Data tab, then click Filter.
    - Click the filter drop-down in column AG (Purchase_Status), and select Filter….
    - In the list, only select Frequent and click OK.
    - Click the filter drop-down in the column AG, and click Clear Filter From “Purchase_Status”.
    - Click the filter drop-down in column AE (T_Type), and select Filter….
    - In the list, only select Cancelled and click OK.
    - Click the filter drop-down in column AF (Purchase_Touchpoint), and select Filter….
    - In the list, only select Desktop and click OK.
    - On the Data tab, click Clear.

    #### To use Custom Filters to filter data:
    - Click the filter drop-down in column AD (Order_Value), then Number Filters>Top 10….
    - Change the value from 10 to 50 and Click OK.
    - Click the filter drop-down in the column AD, and click Clear Filter From “Order_Value”.

  ### Task B: Sorting data
    - On the Data tab, click Custom Sort to open a dialog.
    - Click the Column drop-down of row Sort By, select Order_Ship_Date.
    - Click the Order drop-down of row Sort By, select Sort Ascending.
    - Click Add.
    - Click the Column drop-down of row Then By, select Order_Value.
    - Click the Order drop-down of row Then By, select Sort Descending.
    - Click OK.

# Useful Functions for Data Analysis
  ### Task A: Use of IF to apply one condition
    - Select column AF, right-click, Insert.
    - In cell AF1, type Complete?.
    - In cell AF2, type =IF(AE2="Complete","Yes","No") and press Enter.
    - Double-click the Fill Handle of AF2 to copy down the column.

  ### Task B: Use of Nested IF to apply multiple conditions
    - Select column AE, right-click, Insert.
    - In cell AE1, type Order Size (IFS).
    - In cell AE2, type =IFS(AD2>300,"Large",AD2>100,"Medium",AD2>0,"Small") and press Enter.
    - Double-click the Fill Handle of AE2 to copy down the column.

  ### Task C: Use of IFS to apply multiple conditions (alternative of Nested IF)
    - Select column AE, right-click, Insert.
    - In cell AE1, type Order Size (IFS).
    - In cell AE2, type =IFS(AD2>300,"Large",AD2>100,"Medium",AD2>0,"Small") and press Enter.
    - Double-click the Fill Handle of AE2 to copy down the column.
    
  ### Task D: Use of COUNTIF to count the number of cells that meet a specified criterion
    - Select cell BX2 and type count VISA card.
    - Select cell BY2 and type =COUNTIF(N2:N195,"VISA") and press Enter.

  ### Task E: Use of SUMIF function to sum the values within a specified range that meet a specified criterion
    - Select cell BX3 and type sum Large order.
    - Select cell BY3 and type =SUMIF(AE2:AE195,"Large", AD2:AD195) and press Enter.
        Formula: =SUMIF(range, criteria, [sum range]).

  ### Task F: Use of SUMIFS function to sum the values within a specified range that meet multiple specified criteria
    - Select cell BX4 and type sum Large order with Baby Gen.
    - Select cell BY4 and type =SUMIFS(AD2:AD195, AE2:AE195,"Large", AL2:AL195,"BABY_BOOMERS") and press Enter.
        Formula: =SUMIFS ([sum range], range1, criteria1, range2, criteria2, …).
        


    


