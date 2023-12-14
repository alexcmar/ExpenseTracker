**Expense Tracker**

Description:
    This program allows for an accurate recording of all credit and debit transactions for multiple accounts, provinding multiple summurizing key insights of a person's financial situation, simply by using the transaction csv files provided by one of the supported banks. Currently this program supports the following banks: Caixa Geral de Depósitos (CGD), and Wise. This program uses EUR as a baseline.

Program background:
    This project grew from a need to practice 3 major languages/programs that I had studied in order to keep them fresh in my mind. These were Python, MySQL, and Power BI. Python was used to treat all the data received from the csv files, from data standardization, currency conversion, to actually communicating with the SQL server, amongst other things. MySQL was used to store all the data in several tables that used primary and foreign keys to create a relationship web between them, while SQL use was quite limited due to the use of python libraries such as SQLAlchemy. Power BI served as the end point of the program, allowing user to visualize their data, from a timeline of total financial balance to maps deplaying credits and debits transacted in multiple cities or countries.

Features:  
    - Transaction tracking from 2022-01-01 onwards;  
    - Multiple account tracking;  
    - Automatic currency conversion to EUR;  
    - Ability to assign transactions to specific cities/countries;  
    - Multiple key insights for both a timeline overview and a year/month scale.

Installation:  
    In order to use this program simply download the latest release, unpack the .rar and run the executable file. Please make sure you have the required programs installed on your machine beforehand.

How to use:  
    On the first use, run the executable file, which will allow it to create the necessary folders as well as the database that will be used. After that, you will land on main menu, which will look something like this:  
    Please also note that a new folder "load-in files" was created in the executable's directory and also a new "List of Categories" txt file was created. The folder is where all the transactions files that will be read by the program have to be stored. It also includes a "old files" folder where you can drop files that have already been used. The txt file will be used later, when updating records and it contains all the built-in categories.  
    The main menu contains multiple options to add, edit, or delete data from the database.  
    To add new transaction data to the database, please choose option 2 to update tables, making sure you have a csv file from a supported bank in the "load-in files" folder. This will prompt the user to select a file.  
    NOTE: Please make sure the chosen transaction file does NOT include the current day's date!  
    After choosing a file and if there are no accounts and/or no locations on record, the user will be prompted to add them. The program will then take into account the account chosen, standardizing the csv file based on the account bank, and converting transactions to EUR if necessary. The location chosen is also associated with all transactions.  
    For the main part of the program, the user will be prompted to associate a store/company to each transaction based on its description. If a description is repeated, the program will automatically associate it to the corresponding store on record. After that process, the user will then be prompt to associate each store/company to a category (For reference, the "List of Categories" txt file can be used).  
    On subsequent uses of the program any repeating descriptions will be also be automatically associated with their corresponding stores. Only if new descriptions appear, will the user be prompted to associated them with a store and category.  
    In the main menu, the sub-menus presented give the user the ability to add other categories to the database, delete accounts on record, change the location of a transaction, amongst other things.  
    Finally, to reset the whole database, choose option 9. This will delete the current database and recreate it once again.  
    To visualize the data on record, please use the Power BI template provided in the "Extra files" folder. This template includes for 4 report pages. CTRL+click on the "?" icon in the top left corner to obtain more information about each page.