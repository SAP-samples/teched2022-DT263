# Exercise 1 - Creating an extension of generic report definition

In this exercise, we will learn how to define a document of format "TXT" which would contain the VAT line items

## 1.1 Creating an extended report definition 

1. Click on the "Define Statutory Reports" app 

<img width="1058" alt="Design Time 1" src="https://user-images.githubusercontent.com/115979588/198347215-672fd989-a1e1-43e0-87b9-6c1a62c34d40.png">

2. Go to "Report Definition" tab 

<img width="1440" alt="Screenshot 2022-10-27 at 9 30 19 PM" src="https://user-images.githubusercontent.com/115979588/198347482-65aea90f-843d-4b79-b72d-f89efb35ece7.png">

3. Click on "Add" 
4. Select the radio button "Enhanced" and mark the checkbox "Do you want to extend an existing report definition" 
5. For the "Reference Report Definition" field, use the value-help and choose the report definition "ADV_VAT_RET_SUMMARY".  
   - ADV_VAT_RET_SUMMARY is the generic VAT report definition which is already defined as per the common statutory reporting requirement and can be easily extended. You can read more about such generic reports here: https://blogs.sap.com/2022/07/22/scaling-up-statutory-reporting-with-extensibility-in-sap-s-4hana/ 
6. Enter a meaningful name in the field "New Report Definition" and click on "Continue" 

<img width="1430" alt="Screenshot 2022-10-27 at 9 31 22 PM" src="https://user-images.githubusercontent.com/115979588/198347827-12099aae-dabd-4ff8-bbc9-7d88d8464ac6.png">




## 1.2 Defining a query on the data source which would return the VAT line items 

1. Click on "Edit" 

<img width="1435" alt="Screenshot 2022-10-27 at 9 31 51 PM" src="https://user-images.githubusercontent.com/115979588/198347990-f33f345c-eb88-4ee7-bacf-bfad2d1617bf.png">

2. Step 1 and Step 2 can be skipped as the requirements do not warrant any adjustments here 
3. Under Step 3 - Query Definition, click on "Add" 

<img width="1431" alt="Screenshot 2022-10-27 at 9 32 12 PM" src="https://user-images.githubusercontent.com/115979588/198348121-247f27f6-f752-46fb-9663-2fad607a7f0d.png">

4. Enter a meaningful Query ID and click on continue 

<img width="1440" alt="Screenshot 2022-10-27 at 9 32 29 PM" src="https://user-images.githubusercontent.com/115979588/198348201-ee967062-bd8c-47e6-9cd9-03f8edab86bc.png">

5. Under "General Properties", provide a meaningful description 

<img width="1425" alt="Screenshot 2022-10-27 at 9 33 37 PM" src="https://user-images.githubusercontent.com/115979588/198348290-f9149beb-74f4-49f1-addb-9476aa3a66a8.png">

6. Select the "Data Source Type" as "CDS View" 
7. Search for the CDS view "I_STRPTAXITEM" and select it 

<img width="1414" alt="Screenshot 2022-10-27 at 9 34 14 PM" src="https://user-images.githubusercontent.com/115979588/198350287-7ddc4629-9552-4b92-a31f-451be73df776.png">

8. Under the now visible "Filters" section, set the filters as following: 
   - Search for CompanyCode and set the toggle as true 
   - Under "Define Filter Conditions", Select "Report Parameter", "Equals" from the drop downs and select "CompanyCode" from the "Report Parameter" value- help 
   - Search for "ReportingDate" and repeat the above steps 
   - In the "Report Parameter" value-help, select "Reporting Date" 
   
   <img width="1414" alt="Screenshot 2022-10-27 at 9 34 14 PM" src="https://user-images.githubusercontent.com/115979588/198350522-8b939c11-3262-49c3-b142-32aa343d0529.png">

<img width="1437" alt="Screenshot 2022-10-27 at 9 35 04 PM" src="https://user-images.githubusercontent.com/115979588/198350586-8621c932-47fe-4768-af4b-3d5b4afcaa98.png">

9. Click on "Activate" 

## 1.3 Creating a file/document of format 'TXT' which would contain the VAT line items 

1. Go to Step 4 - Document Definition and click on "Add" and select "Add with schema/query"

<img width="1433" alt="Screenshot 2022-10-27 at 9 35 58 PM" src="https://user-images.githubusercontent.com/115979588/198352233-d792a460-d35c-4a9e-935b-fd0547009100.png">


2. Under "Document Id", provide a meaningful document id 


3. Select "Document Type" as "TXT" and continue 

<img width="1431" alt="Screenshot 2022-10-27 at 9 36 19 PM" src="https://user-images.githubusercontent.com/115979588/198352394-4889f420-74d4-4f4f-964e-203631ccc65b.png">


4. Under "General Properties", provide a meaningful document name 
5. Check the radio button "Create using query" and select the query id created in the previous step 
6. In the "New Schema" pop-up, click on "Select Columns" and in the next pop-up select all the columns and click on "Continue" 

<img width="1433" alt="Screenshot 2022-10-27 at 9 36 59 PM" src="https://user-images.githubusercontent.com/115979588/198352578-cda58223-d17b-4577-8b0e-9a1ff795dec9.png">



<img width="1435" alt="Screenshot 2022-10-27 at 9 37 14 PM" src="https://user-images.githubusercontent.com/115979588/198352924-a51e33c0-7ef3-4cfc-b04e-3d8521b0b21e.png">


<img width="1433" alt="Screenshot 2022-10-27 at 9 37 47 PM" src="https://user-images.githubusercontent.com/115979588/198353002-4ce08247-89f1-4d1f-8b83-3f470f61d5d4.png">


7. Click on "Activate" 

## 1.4 Defining the delimiter ";" 

1. Under "General Properties", in the "Delimiter" field, maintain ";" 

<img width="1428" alt="Screenshot 2022-10-27 at 9 38 10 PM" src="https://user-images.githubusercontent.com/115979588/198353125-1ab7ce4b-af84-462e-899d-12a7c2dff4fa.png">


2. Click on "Activate" 

<img width="1436" alt="Screenshot 2022-10-27 at 9 38 30 PM" src="https://user-images.githubusercontent.com/115979588/198353273-2af711b5-4b56-41de-a84c-15834ad31ea8.png">



## Summary

You have now created an extended report definition which would generate a text file that would contain the VAT line items delimited by ";" 

Continue to - [Exercise 2 - Creating a custom report category](../ex2/README.md)

