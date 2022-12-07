# Blood-Glucose-Log-Book
Final Project BMES 550

Below, provides an overview of each file developed in MATLAB, including  MATLAB's AppDesigner, and DB Browser (SQLite). Note that for someone who wants to run code on their separate device (in WINDOWS) to please install the following 
in each link:

MATLAB https://www.mathworks.com/products/new_products/latest_features.html

DB Browser for SQLite (Standard installer) 
https://sqlitebrowser.org/dl/
__________________________________________________________________________

### NewUser.m
Works by creating a new user database for every new user who registers within the Login.mlapp (GUI). The new user data will be stored within that new user database in DB Browser SQLite.

### ReturnUser.m
After a new user is created, this checks whether a user is actually within the database stored in SQLdatabase browser. This will connect to a new database in DB Browser SQLite so the registry can be stored in the table.

### GetdbFile.m
This is function getdbFile locates the desired file for the callback in gui to connect to SQLdatabase browser.

### SQLdatabase.m
Creates a table of patient data to compile an organize number of each new user's data in stored variables: patientid, username, password, name, age, height, and weight.

### SQLdatabase.db
This contains 2 tables: patient and patient_data. Stored information from new user login's content from Login.mlapp will go into table data.

### Encrypt_decrypt.m
This function prevents clear-text password from being stored in database by encrypting the password, so confidentiality of database is secured.

### Login.mlapp
This is designed to make an interactive environment prompting the user a 'return user' or 'new user' option so user can create a new user login and if user already exists, then access the content of their data by going to return user.

### Homepage.mlapp
After a user passes through the login GUI, it will direct the user to this Homepage GUI. User can interact with the GUI by clicking buttons to access their personalized logbook.

### Main_Menu.mlapp
First tab displays options such as glucose level and date to enter user specific information and see plotted visual of their data. Second tab displays imported information from data entry.
