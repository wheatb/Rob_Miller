# Excel Case Study - Furniture Sales

### **Project Summary**
For this guided project, I portrayed role of a junior data analyst for a furnature company. I was given an unprocessed data file via Excel titled Office Chair Sales as seen in Figure 1. The first outcome of this assignement was to assess two .CSV files for organization and readability. Second, pertinant information regarding sales discounts and price was added to the spreadsheet. The final outcome was to summarize data into one spreadsheet using VLOOKUP allowing for easy accessibility for users. 

The step by step process used for this project is described below.

**Figure 1** The initial .CSV file presented at the start of the project.
![Screenshot (14)](https://user-images.githubusercontent.com/106198562/212751750-790ef8ea-edab-459c-b268-d252bc3e7af3.png)

### Outcome One- Assessing for Organization and Readibility 
Filters were applied to the column headers to improve data accessability within the spreadsheet. Filters include, but are not limited to, customer name, total sales by region, or by total sales per date. After the filters were added, the colors were automatically updated to the spreadsheet, improving the overall readability of the file. 

**Figure 2** The Excel file with added filters.
![0002b](https://user-images.githubusercontent.com/106198562/212759374-258817be-9ad8-44e6-8c6a-5a52b1e0ce8d.jpg)

### Outcome Two- Discount Data Input 
The company used for this project offered a 5% discount if the customer purchased twenty or more chairs. One additional columns was added to the spreadsheet to include information on if the discount was applied. The IF function was applied to the Discount column. This function automatically checks the number of chairs sold in the Number column and applies a Y or N depending if the twenty chair discount condition was met.

**IF Function Code**
`=IF(L5>=20,"Y","N")`

**Figure 3** The Excel file after the Discount column was added and IF function was applied. 
![0003a](https://user-images.githubusercontent.com/106198562/212752860-1925eb4c-7ea2-4ac0-9437-77bf777a4c12.jpg)

Next, I added a Final Price column that reflects the final price of the purchase. An dditiona IF function was added to automatically checks the Number column and applies the discount if the number meets or exceeds twenty. The 5% discount is then automatically reflected in the purchase price column. 

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

Pivot Tables can be applied to this spreadsheet to quickly and easily filter data to create new tables using the PivotTable Field List seen in Figure 7. 

**Figure 7** PivotTable Field List.

![Screenshot (9)](https://user-images.githubusercontent.com/106198562/212741010-5a76ca0d-e9ee-4d78-8ddf-1c5b8920f1b3.png)

Examples of new data tables created using PivotTables are seen below in Figures 8 and 9. 

**Figure 8** Summary of sales by month and sales representive. 

![Screenshot (8)](https://user-images.githubusercontent.com/106198562/212740662-cc69ab7a-15b5-4ceb-8174-10f59789b3e2.png)

**Figure 9** Summary of monthly sales by chair model and sales representative. 
![Screenshot (12)](https://user-images.githubusercontent.com/106198562/212741647-2cf48f82-626d-4865-9d21-5341cbe86c39.png)



