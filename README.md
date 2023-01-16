# Excel Case Study - Furniture Sales

### **Project Summary**
For this guided project, I portrayed role of a junior data analyst for a furnature company. I was given an unprocessed data file via Excel titled Office Chair Sales as seen in Figure 1. The first outcome of this assignement was to assess two .CSV files for organization and readability. Second, pertinant information regarding sales discounts and price was added to the spreadsheet. The final outcome was to summarize data into one spreadsheet allowing for easy accessibility for users.

The step by step process used for this project is described below.

**Figure 1.** The initial .CSV file presented at the start of the project.
![Screenshot (14)](https://user-images.githubusercontent.com/106198562/212751750-790ef8ea-edab-459c-b268-d252bc3e7af3.png)


The first thing I do is apply filters to the data in the spreadsheet to make it both easier to work with as well as easier to read. Our company offers a bulk purchase discount of 5% if the customer purchases 20 or more chairs. Two additional columns are added to make this process automatic, a column to check and see if the order qualifies for the discount, and another column for total price reflecting the discount, if applicaple.


![0002a](https://user-images.githubusercontent.com/106198562/212752802-b969826c-67a8-46b9-ab09-f8a2c92018a0.jpg)

For the first new column, I used the IF function.  It checks the number of sales in the order and returns either Y or N depending on if the condition is met or not. 

`=IF(L5>=20,"Y","N")`

![0003a](https://user-images.githubusercontent.com/106198562/212752860-1925eb4c-7ea2-4ac0-9437-77bf777a4c12.jpg)

Finally I added a final column Total Price that reflects if the discount is or is not applied. 

`=IF(L5>=20,0.95*N5,N5)`

![0007a](https://user-images.githubusercontent.com/106198562/212752987-97fd785b-ff2f-435e-9545-987a6109a588.jpg)

### VLOOKUP

There is a second sheet contining more customer data.  Using VLOOKUP, this data can easily be added to the main sheet.


![0004a](https://user-images.githubusercontent.com/106198562/212753010-c80ca6ba-11ba-43f8-81cb-ec460b673674.jpg)

Added column 'Company Name'
`=VLOOKUP(F5,'Customer Info'!$A$4:$C$12,2,FALSE)`

Added column 'Customer Name'
`=VLOOKUP(F5,'Customer Info'!$A$4:$C$12,3,FALSE)`

![0006a](https://user-images.githubusercontent.com/106198562/212753128-381c21d4-9677-4c9c-8ff7-912a272bbea4.jpg)

### Pivot Tables

With the final data that is now cleaned and re-organized, we can use Pivot Tables to quickly and easily create new tables to summarize our data for us.  I filter the data and create a table showing the sales by sales representative and sales by month.

![Screenshot (9)](https://user-images.githubusercontent.com/106198562/212741010-5a76ca0d-e9ee-4d78-8ddf-1c5b8920f1b3.png)

![Screenshot (8)](https://user-images.githubusercontent.com/106198562/212740662-cc69ab7a-15b5-4ceb-8174-10f59789b3e2.png)

The Pivot Table is able to be expanded even more to show a breakdown of sales by model, for each sales representative.

![Screenshot (12)](https://user-images.githubusercontent.com/106198562/212741647-2cf48f82-626d-4865-9d21-5341cbe86c39.png)



