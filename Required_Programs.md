**Program requirements**  

    - MySQL server version 8.0.28 and MySQL Connector/NET -> https://downloads.mysql.com/archives/community/  
    - Power BI November 23 version or above -> https://www.microsoft.com/en-us/download/details.aspx?id=58494
    - .env file -> Template provided in program folder


**How to install required programs**

    MySQL server and connector:  
        1) Select "No" to the option "Mandatory MySQL Installer Upgrade Available";  
        2) Select "Developer default" in the installation choices or select "Custom" and pick "MySQL Server 8.0.28"
           and "MySQL Connector/NET";  
        3) Press "Execute" to get necessary files;  
        4) While configuring program, choose "Development Computer", and then "Use Legacy Authentication Method";  
        5) Define a password (No need to add a user);  
        6) Complete installation.  
    
    Power BI:  
        1) Simply follow the installation instructions (For first installation or for updating).  
      
    .env file:  
        1. Open template file in a text editor (such as Notepad);  
        2. Replace "<password>" with the server password (Defined when installing MySQL server and connector);  
        3. Save file with "Save as...", change "Save as type" field to "All files", and change name to ".env".  
    
