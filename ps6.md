#### PS6: Due Dec. 2, 2016
---

1. True or False: MySQL automatically creates an _index_ for any key (foreign and primary).
    False- indexes are only automatically created for primary keys and unique constraints, an index must be created for foreign keys.

2. True or False: You can create an index that can improve performance of the database.
    True- they imporove the process of data retrieval.

3. True or False: You should use indexes on columns that return a high percentage of data when that column is used as a filter condition in the `WHERE` clause.
    False

4. True or False:  You should use indexes on columns that have a high number of NULL values.
    False

5. True or False:  You should not use indexes on columns that are frequently manipulated.
    True

6. True or False:  You should never consider indexing a column used in a `GROUP BY` clause.
    False

7. What is a disadvantages of using indexes?
    Sometimes creating indexes slows down data retrieval when use in congruence with 'OR', 'HAVING', 'LIKE', or with sorting, and can't be successfully used with high data main
pulation tables.
8. Decide YES or NO whether an index should be used or not. 
  a. Several columns in a small table
      No
  b. Large table with a lot of data manipulation
      No

9.  Determine which is most restrictive, products in categories 200 or 201 and products manufactured by manufacturer number 72.
    The query determining the manufacturer_id is more restrictive, so in the query it would be placed second so that it would run first throught the database and eliminate more data.
    
10.  Create a VIEW of all products from categories 200 or 201 manufactured by manufacturer 72 or 88. 
      Create view `Question10` as 
      Select Product_id
      From unemath_Rivette.Products
      Where category_id in (200,201) and manufacturer_id in (72,88);
