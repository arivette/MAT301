## Problem Set 4 

1. Create three tables: Customers, Orders, and OrderItems.

2. Why do we need an OrderItems table?

    Because people can order more than one item at a time.

3. Create linked tables in MS Access.
    
    Need MS Access

4. Create forms to enter customer data.

    Need MS Access

5. Create a form with a subform to enter orders and order item.

    Need MS Access

6. Use forms created in 4 and 5 to insert Customers and Orders.  Add customers that have not made any orders. Make the number of entries relatively small.  Why?  

    Need MS Access

7. Use SQL DML to INSERT records into Customers and Orders (and OrderItems).  

    INSERT into unemath_Rivette.Customers (customer_id, customer_first, customer_last, customer_email, customer_phone,
    customer_zip) VALUES (...)
    INSERT into unemath_Rivette.Order (order_id, customer_id, date, time, order_total) VALULES (...)
    INSERT into unemath_Rivette.OrderItems (orderitem_id, product_id, quantity, price) VALUES (...)

8. Find all customer orders.

    SELECT * FROM unemath_Rivette.Orders;

9. Select all customers that orders a certain product (This will depend on what data you entered into the table).  Find all customers that ordered product 3452.  

    SELECT * FROM unemath_Rivette.OrderItems WHERE product_id=3452;

10. List 5 questions that you can answer from this data.

    1. Find all orders that total under $25
    2. Find all customers that have a zipcode of 12804
    3. Find all orders places on 12/24/2015
    4. Find all customer phone numbers who ordered product_id 4509
    5. Find all order totals between $100 and $150 placed between 5:00pm and 6:00pm
