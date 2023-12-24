The files supplied for testing have the following parameters:

    cgd_test.csv: small-sample main account (around 600 transaction rows)
    wise_test.csv: tiny-sample secondary account (around 100 transaction rows)
    main_standard_test: small_sample main account (around 600 transaction rows)
    secondary_standard.csv: tiny-sample secondary account (around 100 transaction rows)

The 2 standard transaction.csv files have the following parameters:

    main_standard_test:
    	Delimiter - ;
    	Load mode - Debits and credits use different columns
    	Date mode - YYYY/MM/DD
    secondary_standard.csv:
    	Delimiter - ;
    	Load mode - Transactions use negative values for debits
    	Date mode - YYYY/MM/DD


The transactions present in the test files all follow the schema below:

    Description - Store - Category
    "Rent" - Rent - 3: Rent
    "Public Transportation Pass" - Public Transportation Pass - 6: Public Transportation
    "Music App" - Music App - 11: Tech/Games/Toys
    "Video Streaming App" - Video Streaming App - 11: Tech/Games/Toys
    "Private Transportation Company" - Private Transportation Company - 7: Private Transportation
    "Restaurant A" - Restaurant A - 9: Restaurants
    "Tech Store" - Tech Store - 11: Tech/Games/Toys
    "Clothes Store" - Clothes Store - 8: Clothes
    "Techlandia" - Techlandia - 11: Tech/Games/Toys
    "Pharmacy" - Pharmacy - 12: Health
    "Clothing 4 All" - Clothing 4 All - 8: Clothes
    "Furniture Store" - Furniture Store - 1: Miscellaneous
    "Online Supermarket" - Online Supermarket - 10: Supermarket
    "Book Store" - Book Store - 1: Miscellaneous
    "TRF P2P" - TRF P2P - 15: P2P transactions
    "Bank Withdrawl" - Bank - 14: Bank transactions
    "Restaurant B" - Restaurant B - 9: Restaurants
    "You Work Here Enterprise" - You Work Here Enterprise - 2: Salary
    "Bank Deposit" - Bank - 14: Bank transactions
