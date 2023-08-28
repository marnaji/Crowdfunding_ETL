# ETL Mini Project
##  Crowdfunding_ETL
In this mini project, tasks encompass producing the Category and Subcategory DataFrames, compiling the Campaign DataFrame, formulating the Contacts DataFrame, and setting up the Crowdfunding Database.

1. Create the Category and Subcategory DataFrames:
    Retrieve and convert the data from the **crowdfunding.xlsx** Excel file to generate a category DataFrame and subcategory DataFrame . 
    * The Category DataFrame encompasses: "category_id" column featuring entries progressing sequentially from "cat1" to "catn",and a "category" column housing exclusively the category titles.
    * The Subcategory DataFrame encompasses : "subcategory_id" column that has entries going sequentially from "subcat1" to "subcatn" , and a "subcategory" column that contains only the subcategory titles. 
Both DataFrames have been exportrd as _category.csv_ and _subcategory.csv_


2. Create the Campaign DataFrame: 
    Extract and convert information from the **crowdfunding.xlsx** Excel dataset to generate a campaign DataFrame with the subsequent columns:
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
The campaign DataFrame has been exported as _campaign.csv_

3. Create the Contacts DataFrame: 
    Extract and transformed the data from **contacts.xlsx**, I used Python dictionary methods and regular expression to perfom the tasks in this section. Both options are working  and extract the data properly. 
    * The contacts DataFrame has been created based on the extracted data. 
    * The column "name" splited into two new columns "first_name" and "last_name" in this DataFrame.
    * Cleaned and export the DataFrame as _contacts.csv_

4. Create the Crowdfunding Database:
    * Inspected four CSV files and the sketch an ERD of the tables by using <a href="https://www.quickdatabasediagrams.com/" target="_blank"> QuickDBD. </a>
    * Used the information from the ERD to create a table schema for each CSV file.
    * Saved the database schema as a Postgres file named crowdfunding_db_schema.sql.
    * Created a new Postgres database, named crowdfunding_db.
    * Used the database schema, create the tables in the correct order to handle the foreign keys.
    * Verified the table creation by running a **SELECT** statement for each table.
    * Imported each CSV file into its corresponding SQL table.
    * Verified that each table has the correct data by running a **SELECT** statement for each.



#### References
Data for this dataset was generated by edX Boot Camps LLC, and is intended for educational purposes only.


