# Excel Case Study - Furniture Sales

### **Project Summary**
For this guided project, I portrayed role of a junior data analyst for a furniture company. I was given an unprocessed data file via Excel titled Office Chair Sales as seen in Figure 1. The first outcome of this assignment was to assess two .CSV files for organization and readability. Second, pertinent information regarding sales discounts and price was added to the spreadsheet. The final outcome was to summarize data into one spreadsheet using VLOOKUP allowing for easy accessibility for users. 

The step by step process used for this project is described below.

**Figure 1** The initial .CSV file presented at the start of the project.
![0001a](https://user-images.githubusercontent.com/106198562/212805577-25dacc12-8531-430d-8851-52d280c52b04.png)

### Outcome One- Assessing for Organization and Readability 
Filters were applied to the column headers to improve data accessibility within the spreadsheet. Filters include, but are not limited to, customer name, total sales by region, or by total sales per date. After the filters were added, the colors were automatically updated to the spreadsheet, improving the overall readability of the file. 

**Figure 2** The Excel file with added filters.
![0002b](https://user-images.githubusercontent.com/106198562/212759374-258817be-9ad8-44e6-8c6a-5a52b1e0ce8d.jpg)

### Outcome Two- Discount Data Input 
The company used for this project offered a 5% discount if the customer purchased twenty or more chairs. One additional columns was added to the spreadsheet to include information on if the discount was applied. The IF function was applied to the Discount column. This function automatically checks the number of chairs sold in the Number column and applies a Y or N depending if the twenty chair discount condition was met.

**IF Function Code**
`=IF(L5>=20,"Y","N")`

**Figure 3** The Excel file after the Discount column was added and IF function was applied. 
![0003a](https://user-images.githubusercontent.com/106198562/212752860-1925eb4c-7ea2-4ac0-9437-77bf777a4c12.jpg)

Next, I added a Final Price column that reflects the final price of the purchase. An additional IF function was added to automatically checks the Number column and applies the discount if the number meets or exceeds twenty. The 5% discount is then automatically reflected in the purchase price column. 

**IF Function Code** `=IF(L5>=20,0.95*N5,N5)`

**Figure 4** The Excel file after the Final Price column was added and IF function was applied. 
![0007a](https://user-images.githubusercontent.com/106198562/212752987-97fd785b-ff2f-435e-9545-987a6109a588.jpg)

### Outcome Three- VLOOKUP

In order to make the data accessible in one spreadsheet, information from the second file titled Customer ID Information was added into two columns in the main spreadsheet. Column G displays the Company Name and Column H lists the Customer Name. The VLOOKUP function was added to the Company and Customer Name columns so the corresponding data would automatically filter into the main spreadsheet. 

**VLOOKUP Function Code added to column 'Company Name'** `=VLOOKUP(F5,'Customer Info'!$A$4:$C$12,2,FALSE)`

**VLOOKUP Function Code added to column 'Customer Name'** `=VLOOKUP(F5,'Customer Info'!$A$4:$C$12,3,FALSE)`

**Figure 5** The Customer ID Information file. 

![0004a](https://user-images.githubusercontent.com/106198562/212753010-c80ca6ba-11ba-43f8-81cb-ec460b673674.jpg)


**Figure 6** The finalized spreadsheet.
![0006a](https://user-images.githubusercontent.com/106198562/212753128-381c21d4-9677-4c9c-8ff7-912a272bbea4.jpg)

### Pivot Tables

Pivot Tables can be applied to this spreadsheet to quickly and easily filter data to create new tables and graphs by using the PivotTable Field List. This list is seen in Figure 7. 

**Figure 7** PivotTable Field List.

![Screenshot (9)](https://user-images.githubusercontent.com/106198562/212741010-5a76ca0d-e9ee-4d78-8ddf-1c5b8920f1b3.png)

Examples of new data tables and graphs created using PivotTables are seen below in Figures 8 and 9.

**Figure 8** Summary table of Monthly Sales by Representative. 

![Screenshot (16)](https://user-images.githubusercontent.com/106198562/212768874-2cd01c15-d440-42c9-bdef-03856cfc5cf9.png)

**Figure 9** Pivot table graph of Monthly Sales by Representative.

![Screenshot (18)](https://user-images.githubusercontent.com/106198562/212769634-a2f7a602-8947-4694-929d-c4bdf5ced99d.png)




