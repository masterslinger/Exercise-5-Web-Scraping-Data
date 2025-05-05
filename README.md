# Exercise-5-Web-Scraping-Data

~~~
Name : W Allen Johnston Ozario  
Reg.No : 21222411004  
~~~

## Aim:
To create a UiPath workflow that scrapes structured data from a website and saves it into a CSV file.

## Materials Required:
UiPath Studio (Community or Enterprise Edition)
Internet connection
A sample website to scrape (e.g., https://www.amazon.com)
Basic knowledge of UiPath's Data Scraping Wizard

## Procedure
 Step 1: Create a New Process
Open UiPath Studio and create a new process named WebScrapingExample.

 Step 2: Open the Target Website
Open your web browser and go to:
[https://www.amazon.com]
 Step 3: Use Data Scraping Wizard
In UiPath Studio, click on "Data Scraping" from the Design tab.

When the wizard opens:

Click on the first product title.

Then click on the second product title to teach the pattern.

When prompted, extract URL as well (optional).

Click Next, then Finish.

The extracted data will be stored in a DataTable variable (e.g., ExtractDataTable).

 Step 4: Write Data to CSV
After the Data Scraping activity, drag a Write CSV activity.

Properties:
  Input: ExtractDataTable
  FilePath: "BooksData.csv" (you can choose your own name)
  Include Headers: ✔️ (checked)

 Step 5: Run the Workflow
 
Save the workflow.
Click Run.

## OUTPUT:
![image](https://github.com/user-attachments/assets/6a713fb8-ea9c-4f36-aa75-8d6adc3734ac)

A CSV file named BooksData.csv will be created in your project folder with data like:

Title	Price	URL
A Light in the Attic	£51.77	http://books.toscrape.com/...
Tipping the Velvet	£53.74	http://books.toscrape.com/...
...	...	...

## Result:
The workflow successfully scrapes data from the website and saves it into a CSV file using UiPath's Data Scraping and File I/O activities.

