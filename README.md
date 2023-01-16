# excel_project_1

For this case study I am working as a junior data analyst for a furnature company.  I am given the following unprocessed data in an Excel File.  

![Raw data](https://user-images.githubusercontent.com/106198562/212725457-a7f73b97-862a-422b-bd37-a5d1fc6be6af.jpg)

The first thing I do is apply filters to the data in the spreadsheet to make it both easier to work with as well as easier to read. Our company offers a bulk purchase discount of 5% if the customer purchases 20 or more chairs. Two additional columns are added to make this process automatic, a column to check and see if the order qualifies for the discount, and another column for total price reflecting the discount, if applicaple.

![0002](https://user-images.githubusercontent.com/106198562/212727731-17fddf0d-5a7a-4c2b-a4ee-b9446eed8f51.jpg)

For the first new column, I used the IF function.  It checks the number of sales in the order and returns either Y or N depending on if the condition is met or not. 
`=IF(L5>=20,"Y","N")`

