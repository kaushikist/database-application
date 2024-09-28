# database-application
Reatil databse application
Online Retail Application Database

Basic outline of the database schema:
Key Points
User Authentication: Ensure secure storage of passwords, possibly using hashing techniques.
Order and Billing: Each order generates a bill based on the quantity, price, and discount of the purchased items.
Relationships: Proper use of foreign keys to maintain data integrity between tables.

Tables and Relationships
1. Users
user_id (Primary Key)
username
password
email
created_at
2. Products
product_id (Primary Key)
name
description
price
stock_quantity
3. Orders
order_id (Primary Key)
user_id (Foreign Key referencing Users)
order_date
total_amount
Order_Items
order_item_id (Primary Key)
order_id (Foreign Key referencing Orders)
product_id (Foreign Key referencing Products)
quantity
price
discount
4. Bills
bill_id (Primary Key)
order_id (Foreign Key referencing Orders)
bill_date
total_amount
