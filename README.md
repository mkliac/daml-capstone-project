# Product Transaction App
This is an application to simulate the product transaction.

### I. Overview
This project was created by using the `empty-skeleton` template. The product owner can create a Product with a price. The owner can update the price, check the price, and most importantly, transfer the ownership to the buyer.
To buy a product from a shop, the user has to create a ShopAccount and deposit money inside. The amount of money in the transaction will be checked before exercising both Deposit and TransferBalance. Again, the owner can check the account balance.

### II. Workflow 
1. Seller creates a product with a price.
2. Buyer deposit money to its account. (amount of deposit must be positive, otherwise -> assertMsg)
3. Buyer transfers money to the seller's account. (amount of transfer money must be positive and less than or equal to balance, otherwise -> assertMsg)
4. Seller transfers the ownership of the product to the buyer.

### Testing
run daml start to check the navigator. 
run daml test to test the script inside 'Test.daml'
