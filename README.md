           REPORTS USING AGGREGATION FUNCTION



Dashboard Link :https://app.powerbi.com/groups/me/reports/fb8f6226-0175-4084-b653-20a5284bb9eb/24ba45846845d233bb91?experience=power-bi



Statement:
Create Reports using Aggregation functions calculate a value such as count, sum, average, minimum or maximum for all rows in a column or table as defined by the expression.

Procedure:
1.	Importing the Dataset:
	Launch Power BI Desktop.
	Click on "Get Data" in the Home tab of the ribbon.
	Select the appropriate data source option "Excel” and follow the prompts to import yoursample dataset into Power BI.

2.	Insert Rectangle Shape:



o	Click on “Format tab” on right side and perform changes on visual.
o	Shape > Style > #E66C37
o	Shape > Text >Text = “Sales report” , Font Size = 46, Horizontal Alignment = “Center”.
 


3.	Add card for Displaying Sum Values of Profit and sales :
	With the card visualization selected, locate the "Fields" pane on the right-hand side.
	Right-click anywhere in the "Fields" pane and select "New Measure" from the contextmenu. This will open the formula bar at the top.
In the formula bar, enter the following DAX formula to create a measure that calculatesthe total profit and sales.
TotalProfit = CALCULATE(SUM(ORDERS[PROFIT]))
TotalSales = CALCULATE(sum(Orders[Sales]))
	Press Enter to apply the formula.
	Visualization >Format Visual > General > Effects > Background Color : #E6E6E6
	Visualization > Format Visual >Visual > Category Label > Font Size = 12 Output:

 
Similarly, calculate the individual years total profit by using the below formulas:
•	2020Profit = CALCULATE(SUM(ORDERS[PROFIT]),year(Orders[Order Date])=2020)
•	2020Profit = CALCULATE(SUM(ORDERS[PROFIT]),year(Orders[Order Date])=2020)
•	2020Profit = CALCULATE(SUM(ORDERS[PROFIT]),year(Orders[Order Date])=2020)
•	2020Profit = CALCULATE(SUM(ORDERS[PROFIT]),year(Orders[Order Date])=2020)
Similarly, calculate the individual years total sales by using the below formulas:
	2020sales = calculate(sum(Orders[Sales]),year(Orders[Order Date])=2020)
	2020sales = calculate(sum(Orders[Sales]),year(Orders[Order Date])=2020)
	2020sales = calculate(sum(Orders[Sales]),year(Orders[Order Date])=2020)
	2020sales = calculate(sum(Orders[Sales]),year(Orders[Order Date])=2020)


4.	Add card for Displaying Average Values of Profit and sales :
	With the card visualization selected, locate the "Fields" pane on the right-hand side.
	Right-click anywhere in the "Fields" pane and select "New Measure" from the contextmenu. This will open the formula bar at the top.
	In the formula bar, enter the following DAX formula to create a measure that calculatesthe avearge profit and sales
avgprofit = CALCULATE(AVERAGE(Orders[profit])) avgsales = CALCULATE(AVERAGE(Orders[Sales]))
	Press Enter to apply the formula.
	Visualization >Format Visual > General > Effects > Background Color : #B6E6E6
	Visualization > Format Visual >Visual > Category Label > Font Size = 12

Output:
 	 

Similarly, calculate the individual years average profit by using the below formulas:
•	2020avgProfit = CALCULATE(AVERAGE(ORDERS[PROFIT]),year(Orders[Order Date])=2020)
•	2021avgProfit = CALCULATE(AVERAGE(ORDERS[PROFIT]),year(Orders[Order Date])=2021)
•	2022avgProfit = CALCULATE(AVERAGE(ORDERS[PROFIT]),year(Orders[Order Date])=2022)
•	2023avgProfit = CALCULATE(AVERAGE(ORDERS[PROFIT]),year(Orders[Order Date])=2023)

Similarly, calculate the individual years average sales by using the below formulas:
•	2020avgsales = CALCULATE(AVERAGE(Orders[Sales]),year(Orders[Order Date])=2020)
•	2021avgsales = CALCULATE(AVERAGE(Orders[Sales]),year(Orders[Order Date])=2021)
•	2022avgsales = CALCULATE(AVERAGE(Orders[Sales]),year(Orders[Order Date])=2022)
•	2023avgsales = CALCULATE(AVERAGE(Orders[Sales]),year(Orders[Order Date])=2023)


5.	Add card for Displaying count of items and orders:
	With the card visualization selected, locate the "Fields" pane on the right-hand side.
	Right-click anywhere in the "Fields" pane and select "New Measure" from the contextmenu. This will open the formula bar at the top.
	In the formula bar, enter the following DAX formula to create a measure that calculatesthe no of items and orders
totalItems = CALCULATE(sum(orders[quantity])) TotalOrders = CALCULATE(COUNT(Orders[Order ID]))
Press Enter to apply the formula.
	Visualization >Format Visual > General > Effects > Background Color : #E6F2g6
	Visualization > Format Visual >Visual > Category Label > Font Size = 12

Similarly, calculate the individual years orders by using the below formulas:
•	2020OrderCount = CALCULATE(count(Orders[Order ID]),year(Orders[Order Date])=2020)
•	2021OrderCount = CALCULATE(count(Orders[Order ID]),year(Orders[Order Date])=2021)
•	2022OrderCount = CALCULATE(count(Orders[Order ID]),year(Orders[Order Date])=2022)
•	2023OrderCount = CALCULATE(count(Orders[Order ID]),year(Orders[Order Date])=2023)

Output:
Similarly, calculate the individual year items by using the below formulas:
•	2020items = calculate(sum(Orders[Quantity]),year(Orders[Order Date])=2020)
•	2021items = calculate(sum(Orders[Quantity]),year(Orders[Order Date])=2021)
•	2022items = calculate(sum(Orders[Quantity]),year(Orders[Order Date])=2022)
•	2023items = calculate(sum(Orders[Quantity]),year(Orders[Order Date])=2023)

 
6. Final Output


![Image](https://github.com/user-attachments/assets/24e40c7d-d1d0-41b4-ad82-590b15d63b4d)
