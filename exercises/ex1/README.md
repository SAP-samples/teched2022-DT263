# Exercise 1 - Creating an extension of generic report definition

In this exercise, we will learn how to define a document of format "TXT" which would contain the VAT line items

## 1.1 Creating an extended report definition 

1. Click on the "Define Statutory Reports" app 
2. Go to "Report Definition" tab 
3. Click on "Add" 
4. Select the radio button "Enhanced" and mark the checkbox "Do you want to extend an existing report definition" 
5. For the "Reference Report Definition" field, use the value-help and choose the report definition "ADV_VAT_RET_SUMMARY".  
   - ADV_VAT_RET_SUMMARY is the generic VAT report definition which is already defined as per the common statutory reporting requirement and can be easily extended. You can read more about such generic reports here: https://blogs.sap.com/2022/07/22/scaling-up-statutory-reporting-with-extensibility-in-sap-s-4hana/ 
6. Enter a meaningful name in the field "New Report Definition" and click on "Continue" 



## 1.2 Defining a query on the data source which would return the VAT line items 

1. Click on "Edit" 
2. Step 1 and Step 2 can be skipped as the requirements do not warrant any adjustments here 
3. Under Step 3 - Query Definition, click on "Add" 
4. Enter a meaningful Query ID and click on continue 
5. Under "General Properties", provide a meaningful description 
6. Select the "Data Source Type" as "CDS View" 
7. Search for the CDS view "I_STRPTAXITEM" and select it 
8. Under the now visible "Filters" section, set the filters as following: 
   - Search for CompanyCode and set the toggle as true 
   - Under "Define Filter Conditions", Select "Report Parameter", "Equals" from the drop downs and select "CompanyCode" from the "Report Parameter" value- help 
   - Search for FiscalPeriod and repeat the above steps 
   - In the "Report Parameter" value-help, select "Reporting Date" 
9. Click on "Activate" 


## Summary

You have now created an extended report definition which would generate a text file that would contain the VAT line items delimited by ";" 

Continue to - [Exercise 2 - Creating a custom report category](../ex2/README.md)

