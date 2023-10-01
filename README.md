# EasyIMPORT - Google Sheets Extension

## Overview

EasyIMPORT is a Google Sheets extension that simplifies the process of importing CSV data column wise into your Google Sheets documents. It also allows you to filter the data before importing it. 

## Features

- Import CSV data directly into Google Sheets.
- Customize the import by selecting specific columns.
- Apply filters to the data before importing.

## Installation

### Prerequisites

Before you begin, make sure you have the following:

- A Google account.
- Access to Google Sheets.
- A GCD account to use the Add-on

### Installation Steps

1. Open your Google Sheets document.
2. Click on "Extensions" in the top menu.
3. Choose "Apps Script."
4. copy paste the Code.gs
5. Make a new HTML file by the name Sidebar.html and copy paste the html code there.
6. Select Deploy -> New Deployment -> select type -> Add-on -> give a description for it and deploy!
7. If making add-on for the first time, go to project settings -> Google Cloud Platform (GCP) Project -> Project Number(make a new one from your GCD account)
8. GoogleSheets will open, resfesh it and after waiting for 1-2 mins, the add-on would become available in extension tab!

## Usage

### Importing CSV Data

To import CSV data into your Google Sheets document:

1. Click on the "EasyIMPORT" menu from extension tab.
2. Drag and drop your .CSV into the box.
3. Or select "Import CSV."
4. Choose a CSV file from your computer.
5. Select the columns you want to import.
7. Click "Import."

### Filtering Data

Before importing data, you can apply filters:

1. Click on the "EasyIMPORT" menu.
2. Select "Filter Data."
3. Choose a filter column and enter a filter value.
4. Click "Apply Filter."
5. Now, when you import data, only matching rows will be imported.
   
## Web Page

In addition to the Google Sheets add-on, I have also created a dedicated web page for EasyIMPORT. You can access it at [https://www.easyimport.com](https://www.easyimport.com) .

## Acknowledgments

This extension uses the [PapaParse library](https://github.com/mholt/PapaParse) for CSV parsing.

## Screenshots
![image1](https://github.com/ananya-singh-baghel/EasyIMPORT/assets/76189053/66ce986c-3656-4065-9399-795eb65f1a40)

![logo2](https://github.com/ananya-singh-baghel/EasyIMPORT/assets/76189053/e803903d-7930-46ba-9261-1f2e1e74085a)


## Roadmap

I had an idea after reading the problem statment that this assigment will require me doing a lot of research, Due to me not having much prior experience in deployement of extensions, it was a big blocker to me to get my hands on right resourses, learn and then start making this add-on from scratch. Initially I decided on making a web app as that is something i was very famaliar with, so I started the coding for same. At the same time during the whole process of figuring out the App Script feature of Google Sheets I came across this documentation [Script Documentation](https://developers.google.com/apps-script/samples/automations/import-csv-sheets#:~:text=To%20view%20the%20created%20files,select%20updateApplicationSheet%20and%20click%20Run) , which made me famaliar with the add-on feature of google sheets! It helped me alot in understanding the basics and putting up a foundation of this project. After going to much research I understood the difference between add-on creation (Ui creation) and web app creation (doGet function) and what are the pre requisites to chnage my web app to an add-on. 

After completing the coding part of the web app, I trial ran it through different type of test cases, for better performance with large .CSV I also implemented batch processing in my code! Afterwards I further went on towards Add-on creation and reused 95% of my web app code for the same, just changing doGet function with a new the Ui creator function. 

Finally there were some touch ups and adjustments required to the CSS of the add-on. I ran the very same test cases for the add-ons too to make sure that the csv data is being parsed correctly and the overall working is up to the mark.
