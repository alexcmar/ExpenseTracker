**Expense Tracker**
~~~
Description:
    
    This program allows for an accurate recording of all credit and debit transactions for multiple accounts, providing multiple summarizing key insights of a person's financial situation simply by using the transaction files provided by one of the supported banks. Currently this program supports the following banks: Caixa Geral de Depósitos (CGD), Activobank, and Wise. This program also allows for various currencies to be used as a baseline, converting all transactions that use other currencies.
    The dashboard provided includes the following 4 report pages:
        - Overview: This page contains broad information regarding all accounts;
        - Credits / Debits: This page contains information regarding all credit and debit transactions recorded;
        - Year: This page contains all information for the selected year, including the savings rate, and a map of transaction locations;
        - Month: This page contains all information for the selected month, including a gauge for expenditure control, based on how much the user wants to save.
    As of version 3.0.0, the Expense Tracker program's source code has also been made available as part of the release package.
~~~
    Program background:
    
        This project grew from a need to practice 3 programming languages/programs that I had studied in order to keep them fresh in my mind. These were Python, MySQL, and Power BI. Python was used to treat all the data received from the transaction files, from data standardization to currency conversion and communication with the SQL server, through the SQLAlchemy library, amongst other things. MySQL was used to store all data in several tables, using primary and foreign keys to create a relationship web between them. Power BI served as the endpoint of the program, allowing the user to visualize the data, from a timeline of total financial balances to maps displaying credits and debits transacted in multiple cities or countries.
~~~
Features:
    
    - Transaction tracking from 2022-01-01 onwards;
    - Multiple account tracking;
    - Automatic currency conversion to the selected baseline currency;
    - Ability to assign transactions to specific cities/countries;
    - Multiple key insights for both a timeline overview and a year/month scale.
~~~
    Installation:
    
        In order to use this program, simply download the latest release, unpack the .rar and run the executable file. Please check the "Required Programs" file to make sure all the required programs are properly installed on your machine beforehand.
        NOTE: If a previous version was being used, please check if an update file has been provided. Be sure to run it before using the newest version of the program.
~~~
How to use:

    The first time, run the executable file, which will allow the program to create all necessary folders as well as the database that will be used. After that, you will land on the main menu.
    Please also note that a new folder "load-in files" will be created in the executable's directory as well as a new "List of Categories" text file. The folder will be used as a root directory for all transaction files. It also includes an "old files" folder where you can drop files that have already been used. The "List of Categories" text file can be consulted when updating records.

    The first time, the user will also be prompted to add their desired base currency. All transaction and balance amounts will be converted to this currency, using the transaction day's conversion rate.

    The main menu contains multiple options to add, edit, or delete data from the database.
    To add new transaction data to the database, please choose option 2 to update tables, making sure you have a compatible transaction file from a supported bank (or a standardized file) in the "load-in files" folder.

    If there are no accounts and/or no locations on record, the user will be prompted to add them before choosing which transaction file to use. The program will then take into account the account chosen, standardizing the file based on the account's bank, converting transactions to the base currency if necessary. The location chosen is also associated with all transactions present on the file.

    For standardized (from non-acceptable banks) files, the user will be asked for the delimiter used in the file, the load mode of the file (if debit transactions appear as negative values, or if credits and debits use different columns), and the date format used by the file.

    For the main part of the program, the user will be prompted to associate a store/company with each transaction based on its description. If a description is repeated, the program will automatically associate it with the corresponding store on record.
    Afterwards, the user will then be prompted to associate each store/company with a broad category (the "List of Categories" text file can be used for reference).

    On subsequent uses of the program, any repeating descriptions will also be automatically associated with their corresponding stores. Only new descriptions will prompt the user to associate them with a store and category.

    In the main menu, the sub-menus presented give the user the ability to add other categories to the database, delete accounts on record, and change the location of a transaction, amongst other things.
    If a database reset is required, choose option 9. This will delete the current database and recreate it once again, without any transactions. All transactions will need to be reentered by the user. 

    To visualize the data on record, please use the Power BI template provided in the "Extra files" folder. This template includes 4 report pages.
        - Overview: This page contains broad information regarding all accounts;
        - Credits / Debits: This page contains information regarding all credit and debit transactions recorded;
        - Year: This page contains all information for the selected year, including the savings rate, and a map of transaction locations;
        - Month: This page contains all information for the selected month, including a gauge for expenditure control, based on how much the user wants to save.
    
    CTRL+clicking on the "?" icon in the top left corner displays more information about each page.
