# ETL Mini Project
##  Crowdfunding_ETL
In this mini project, tasks encompass producing the Category and Subcategory DataFrames, compiling the Campaign DataFrame, formulating the Contacts DataFrame, and setting up the Crowdfunding Database.

1. Create the Category and Subcategory DataFrames:
    Retrieve and convert the data from the <b crowdfunding.xlsx /b> Excel file to generate a category DataFrame and subcategory DataFrame . 
    * The Category DataFrame encompasses: "category_id" column featuring entries progressing sequentially from "cat1" to "catn",and a "category" column housing exclusively the category titles.
    * The Subcategory DataFrame encompasses : "subcategory_id" column that has entries going sequentially from "subcat1" to "subcatn" , and a "subcategory" column that contains only the subcategory titles. 
Both DataFrames have been exportrd as <i category.csv /i> and <i subcategory.csv /i>


2. Create the Campaign DataFrame: 
    Extract and convert information from the <b crowdfunding.xlsx /b> Excel dataset to generate a campaign DataFrame with the subsequent columns:
    * The "cf_id" column
    * The "contact_id" column
    * The "company_name" column
    * The "blurb" column, renamed to "description"
    * The "goal" column, converted to the float data type
    * The "pledged" column, converted to the float data type
    * The "outcome" column
    * The "backers_count" column
    * The "country" column
    * The "currency" column
    * The "launched_at" column, renamed to "launch_date" and with the UTC times converted to the datetime format
    * The "deadline" column, renamed to "end_date" and with the UTC times converted to the datetime format
    * The "category_id" column, with unique identification numbers matching those in the "category_id" column of the category DataFrame
    * The "subcategory_id" column, with the unique identification numbers matching those in the "subcategory_id" column of the subcategory DataFrame
The campaign DataFrame has been exported as <i campaign.csv /i>

3. Create the Contacts DataFrame: 
    Extract and transformed the data from <b contacts.xlsx /b>, I used Python dictionary methods and regular expression to perfom the tasks in this section. Both options are working  and extract the data properly. 
    * The contacts DataFrame has been created based on the extracted data. 
    * The column "name" splited into two new columns "first_name" and "last_name" in this DataFrame.
    * Cleaned and export the DataFrame as <i contacts.csv /i>

4. Create the Crowdfunding Database:





