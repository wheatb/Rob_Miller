# Excel Case Study - Furniture Sales

For this guided project, I am playing the role of a junior data analyst for a furnature company. I am given the following unprocessed data in an Excel File titled Office Chair Sales. The purpose of this assignement is to assess the data for organization and readability, apply functions to  

![Screenshot (14)](https://user-images.githubusercontent.com/106198562/212751750-790ef8ea-edab-459c-b268-d252bc3e7af3.png)


The first thing I do is apply filters to the data in the spreadsheet to make it both easier to work with as well as easier to read. Our company offers a bulk purchase discount of 5% if the customer purchases 20 or more chairs. Two additional columns are added to make this process automatic, a column to check and see if the order qualifies for the discount, and another column for total price reflecting the discount, if applicaple.

![0002](https://user-images.githubusercontent.com/106198562/212727731-17fddf0d-5a7a-4c2b-a4ee-b9446eed8f51.jpg)

For the first new column, I used the IF function.  It checks the number of sales in the order and returns either Y or N depending on if the condition is met or not. 

`=IF(L5>=20,"Y","N")`

![0003](https://user-images.githubusercontent.com/106198562/212728877-46302f10-32b0-45c1-a060-0a0313fe9692.jpg)

Finally I added a final column Total Price that reflects if the discount is or is not applied. 

`=IF(L5>=20,0.95*N5,N5)`

![0007](https://user-images.githubusercontent.com/106198562/212730604-3f206f67-c591-43e4-8917-81e9d4529540.jpg)

### VLOOKUP

There is a second sheet contining more customer data.  Using VLOOKUP, this data can easily be added to the main sheet.


![0004](https://user-images.githubusercontent.com/106198562/212730851-d73d0260-f134-4d0a-ad9b-eef056e6bc1a.jpg)

Added column 'Company Name'
`=VLOOKUP(F5,'Customer Info'!$A$4:$C$12,2,FALSE)`

Added column 'Customer Name'
`=VLOOKUP(F5,'Customer Info'!$A$4:$C$12,3,FALSE)`


![0006](https://user-images.githubusercontent.com/106198562/212731777-041c6b8c-ea53-4c08-b677-cb09ebe2c756.jpg)

### Pivot Tables

With the final data that is now cleaned and re-organized, we can use Pivot Tables to quickly and easily create new tables to summarize our data for us.  I filter the data and create a table showing the sales by sales representative and sales by month.

![Screenshot (9)](https://user-images.githubusercontent.com/106198562/212741010-5a76ca0d-e9ee-4d78-8ddf-1c5b8920f1b3.png)

![Screenshot (8)](https://user-images.githubusercontent.com/106198562/212740662-cc69ab7a-15b5-4ceb-8174-10f59789b3e2.png)

The Pivot Table is able to be expanded even more to show a breakdown of sales by model, for each sales representative.

![Screenshot (12)](https://user-images.githubusercontent.com/106198562/212741647-2cf48f82-626d-4865-9d21-5341cbe86c39.png)



