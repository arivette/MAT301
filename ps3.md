## Problem Set 3 

1. Define the terms: relation, tuple, attribute, record, and field.

  - A relation is a table
  - A tuple is a row of a relation (table)
  - An attribute is a column of a relation (table)
  - A record is a row is a tuple
  - A field is a column is an attribute
  
      __Correct__




2. What are keys in a relation?

  - Keys are one or more attribute in a relation used to identify a record, keys can be unique or nonunique
  
      __Correct__




3. What is a surrogate key and how is it used?

 - A surrogate key is a column made by an arbitrary assignment of a key to a row, and is used as an alternative for natural keys which can change or become obsolete, like how a social security number should be unique to every person on the planet but is not always so or can change.
 
 
     __Correct__




4. In the following equation, Area = Length x Width, identify the determinant(s).

 - Determinants are length and width
 
 
     __Correct__




5. If a relation has no duplicate data, how can you be sure there is always at least one primary key?

 - Because the collection of all the attributes in the relation can identify a unique row
 
     __Correct__




6. Give an example of a relation.  Determine a natural key for this relation.

 - An example of a relation would be a table with first name, last name, and address.
 
     __Correct__




 For question 7 - 8, Consider product *orders*.  In particular, associated with an order is: customer name (first and last), address (street, city, state, zip), phone, email, the products orders (including item, quantity, and price). 

7. Create a relational data model for *orders*.  Consider applying normalization rules (discuss Monday)

  - Customers (cust_id [pk], first_name, last_name, phone, address {street, city, state, zip[fk]}, email, orders)
  - Orders (order_id [pk], cust_id [fk], date)
  - Zip (zip [pk], city, state)
  - Products (product_id [pk], msrp)
  - Order_info (order_info_id [pk], product_id [fk], quantity)
  
      __Order info table should have order_id__




8. For customer, could email be used as a primary key?  If so, state why.  Also, if possible to use as a primary key, discuss any disadvantages of using email as a primary key.

  - Yes, because no two people can have the same email, however people can change their email or have multiple email addresses.


    __Correct__



9. Given two relations S and R below find the Cartsian Product S x R. 

| A | B | C | D | E |
|---|---|---|---|---|
| 1 | 2 | 3 | 1 | 1 |
| 2 | 3 | 2 | 2 | 3 |
| 0 | 0 | 2 | 1 | 5 |

    __X__


10 . Find the natural join between the Faculty and Department relations below.

  - The natural join is department

    __Correct__



S
--------------
| A | B |
|---|---|
| 1 | 2 |
| 2 | 3 |
---------

R
------------
| C | D | E |
|---|---|---|
| 3 | 1 | 1 |
| 2 | 2 | 3 |
| 2 | 1 | 5 |



Faculty
--------------
| Name | ID | Dept |
|-------|----|----------------|
| Joe | 1 | Chemistry |
| Susan | 2 | Math |
| Tom | 3 | Marine Science |
| Mike | 4 | Math |


Department
------------
| Dept | Chair  |
|---|---|
| Chemistry | John |
| Math | Mike |
| Marine Science | Barry |
