# E-commerce-Sales-Dashboard-Business-Analytics-with-Excel

Step 1: Create Histogram for Shipping Days (Aging).
Click the Data Tab, Under Analysis Group, Click Data Analysis. select Histogram. In the histogram dialog box, first click the Label’s Check box as we have labels in our data. 
In the Input Reference box, select the range sales and in the Bin Range Reference box Select Bin.
In Output section, select range N3 for binning table.

Step 2: Create Combo Box: 
Insert Combo box for product category list in the Dashboard Sheet.
Click Developer Tab > Under Controls Panel > Click Combo box and draw.
Pass the Input Range and Cell for the Combo box.
Right-click the country list Combo box > Click Format Control > Under Format Control Panel, Pass Input Range “Working!Q2:Q5” and Cell Link “Working!R2” from the working sheet.
Now, write the offset function in cell “R3” to fetch the product category based on the selection in the product category Combo box.

Step3: SUMIFS formula to calculate Total Sales, Quantity, and Profit
Cell C7: =sumifs(‘Sales Data’!$H:$H, ‘Sales Data’!$F:$F, Working!$R$3)
Cell G7: =sumifs(‘Sales Data’!$I:$I, ‘Sales Data’!$F:$F, Working!$R$3)
Cell K7: =sumifs(‘Sales Data’!$K:$K, ‘Sales Data’!$F:$F, Working!$R$3)

Step 4: SUMIFS formula to calculate Sales and Profit month wise
Now write the sumifs formula to calculate the Sales and profit month-wise and sales region-wise. 
Enter formula in Cell C4: =sumifs(‘Sales Data’!H:H, ‘Sales Data’!U:U’, ‘$B$4’, Data!F:F,’$R$3’)
Now, copy and paste the formula in Range C4:C15.
Enter formula in Cell D4: =sumifs(‘Sales Data’!K:K’, ‘Sales Data’!U:U’,’ $B$4’, ‘Data!F:F’, ‘$R$3’)
Now, copy and paste the formula in Range D4:D15.


Step 5: SUMIFS formula to calculate Sales region wise
=sumifs(‘Sales Data’!H:H’, ‘Sales Data’!T:T’, ‘$F$4’, ‘Data!F:F’, ‘$R$3’)
Now, copy and paste the formula in Range G4:G15.
Step 6: Create Column Chart
Now, create the column chart for both region-wise and month-wise table.
Select table (B3:D15), click insert tab > under Charts Panel > Insert column chart and make a presentable Dashboard.







