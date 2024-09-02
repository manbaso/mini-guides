# Importing the Sakila MySQL Sample Database

This documentation provides a step-by-step guide for downloading, extracting, and importing the Sakila MySQL sample database into MySQL Workbench. The Sakila database is a popular sample database provided by MySQL, used for learning and demonstration purposes.

## Prerequisites
Before you begin, ensure you have the following:

- MySQL Workbench: Installed on your machine.
- Internet Access: To download the Sakila sample database.

### STEP 1: Download the Sakila Database

Begin by downloading the Sakila MySQL sample database. You can download it from the official MySQL website. The download will be in a compressed (zip) format.

#### -----

        https://dev.mysql.com/doc/index-other.html

### STEP 2: Download the ZIP File

After navigating to the download page, locate and click on the "Zip" option to download the Sakila database in a compressed format. This will save the file to your default download directory.

#### -----

![sakila 1](https://github.com/user-attachments/assets/7e279590-4e47-4b72-8e2e-124247595185)

### STEP 3: Extract the ZIP File

Once the download is complete, navigate to the directory where the file was saved. Right-click on the zip file and select "Extract All" to begin extracting the contents of the file.

#### -----

![sakila 2](https://github.com/user-attachments/assets/0fdf4188-d85a-41bc-8e9a-5c9f30d76e74)

### STEP 4: Complete the Extraction

A prompt will appear asking where to extract the files. Simply click "Extract" to extract the files to the default location or specify a different location if needed.

#### -----

![sakila 3](https://github.com/user-attachments/assets/b6944d18-a7b7-4633-b1a0-9776e8fbe30c)

### STEP 5: Verify the Extraction

After the extraction process is complete, confirm that a folder named sakila has been created in the same location as the downloaded zip file. This folder contains the SQL scripts required to create and populate the database.

#### -----

![sakila 4](https://github.com/user-attachments/assets/7a611c78-71c1-4f48-a7b1-2876a551a952)

### STEP 6: Open MySQL Workbench

Now, open MySQL Workbench, which you will use to import the Sakila database. You can do this by searching for "MySQL Workbench" in the Windows search box or by locating it in your installed programs. 

#### -----

![sakila 5](https://github.com/user-attachments/assets/da5035db-6a81-4541-a0dd-081bfb43ea5c)

### STEP 7: Connect to the MySQL Server

In MySQL Workbench, select an existing connection to connect to your MySQL server. If you do not have any connections set up, you may need to create one. Typically, you can use a "local" connection if MySQL is installed locally on your machine.

#### -----

![sakila 6](https://github.com/user-attachments/assets/acdca308-a814-4c0d-a1da-89e0f9063d1a)

### STEP 8: Drop the Existing Sakila Database (If Any)

If a previous version of the Sakila database exists, you may want to remove it before importing the new one. Enter the following SQL commands into the query tab:

#### -----

        drop sakila;
    
        show databases;

Click the "Execute query" icon, which is highlighted in yellow in the screenshot, to run the commands. This will drop the existing Sakila database and show all databases currently on your MySQL server.

![sakila 7](https://github.com/user-attachments/assets/dc1c4a17-a131-49ee-981b-aec4553818c8)

### STEP 9: Open the SQL Script for the Sakila Schema

Next, you will need to import the schema for the Sakila database. Click on the "Open a SQL script file in a new query tab" icon, highlighted in yellow, to open the schema file.

#### -----

![sakila 8](https://github.com/user-attachments/assets/032d7646-1cb2-414f-aec8-76739af65ada)

### STEP 10: Select the Sakila Schema File

Navigate to the location where the Sakila folder was extracted. Inside this folder, you will find a file named sakila-schema.sql. Double-click on this file to open it in MySQL Workbench.

#### -----

![sakila 9](https://github.com/user-attachments/assets/5d5d93de-3654-43d6-bfb6-e03788c98c6d)

### STEP 11: Execute the Sakila Schema Script

With the sakila-schema.sql file open, click on the "Execute query" icon, highlighted in yellow, to run the script. This will create the necessary database structure (tables, views, etc.) for Sakila in your MySQL server.

#### -----

![sakila new](https://github.com/user-attachments/assets/c9447043-a43a-4483-a901-5417f28b55e9)

### STEP 12: Open the SQL Script for Sakila Data

After creating the schema, you need to populate the Sakila database with data. Click on the "Open a SQL script file in a new query tab" icon again to open the data script.

#### -----

![sakila 8](https://github.com/user-attachments/assets/032d7646-1cb2-414f-aec8-76739af65ada)

### STEP 13: Select the Sakila Data File

Navigate back to the Sakila folder and select the sakila-data.sql file. Double-click this file to load its contents into a new query tab in MySQL Workbench..

#### -----

![sakila 12](https://github.com/user-attachments/assets/a4bdaa43-3fc8-4cde-be73-813bc69b2620)

### STEP 14: Execute the Sakila Data Script

Click the "Execute query" icon, highlighted in yellow, to run the data script. This script will populate the Sakila database with sample data, such as movies, actors, and rental records.

#### -----

![sakila 13](https://github.com/user-attachments/assets/997aeffd-6f32-41ed-8063-4a45bf52ad2b)

### Step 15:  Verify the Sakila Database

To verify that the Sakila database was successfully imported, open a new SQL query tab by clicking the icon highlighted in yellow.

#### -----

  ![sakila new2](https://github.com/user-attachments/assets/124e46e9-409c-49e6-8a31-e0adb2f3913d)

### STEP 16: List All Databases

In the new query tab, enter the following SQL command to list all databases:

#### -----

          show databases
  
Click the "Execute query" icon, highlighted in yellow, to run the command. You should see sakila listed among the databases, confirming that the import was successful.

![sakila 15](https://github.com/user-attachments/assets/e7212c53-0963-46a0-a3bb-36094cbe1a72)

### STEP 17: List All Tables in the Sakila Database

Next, switch to the Sakila database and list all its tables. Clear the query panel and enter the following commands:

#### -----

  Clear the query panel and paste the following queries:

          use sakila
        
          show tables

Click the "Execute query" icon, highlighted in yellow, to run the commands. This will display all the tables within the Sakila database, confirming that the schema was correctly set up.

![sakila 16](https://github.com/user-attachments/assets/d0d3f59c-c898-42cf-8120-28b9d7f84ea4)

### STEP 18: Query the Sakila Database

Finally, let's run a sample query to ensure the data was imported correctly. Clear the query panel and enter the following command:

#### -----

Clear the query panel and paste the following query:

          select * from actor

Click the "Execute query" icon, highlighted in yellow, to run the query. This will return all records from the actor table, providing a sample of the available data in your Sakila database.
  
![sakila 17](https://github.com/user-attachments/assets/686a2698-b47f-4727-9fe5-7e3666d5ab0b)


















