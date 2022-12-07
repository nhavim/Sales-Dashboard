# Sales-Dashboard
Analyzing sales data in Power Bi
1. open the Power Bi app and click G0et data to upload the Excel file.
2. Specicifically upload location, people, product and sales tables.
3. Create data mode between the tables. Click on data model on the left side of the canvas.
4. Drag Geo under location table unto geography under sales table to create a relationship between the four table.
5. Click on view report 

# Visualizing sale by location
. Click on column bar. Drag Geo under location to X-axis and drag Amount under the sales table to the Y-axis

# Total sale
Select sales and click on amount and select New measure. Enter "Total Sales = sum(sales[Amount]) then enter.
# Total Cost 
First calculate Cost. Go to data view and slect, click on Table tools at the top and select New Measure. Enter Cost = sales[Boxes] * RELATED (products[Cost per box]) and enter.
Repeat the process Total Cost and enter Total Cost = sum(sales[Cost]).
# Total Profit
Create New Measure enter Total Profit = [Total Sales]-[Total Cost].
Repeat the steps and enter Profit% = divede ([Total Profit], [Total Sales])

# Profit Target 
Create new measure, enter Profit Target Achieve? = if ([Profit%])>0.5, "Yes", "No")

now you you all together and display on the dashboard.