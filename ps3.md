## Problem Set 3 

1. Define the terms: relation, tuple, attribute, record, and field.

  - A relation is a table
  - A tuple is a row of a relation (table)
  - An attribute is a column of a relation (table)
  - A record is a row is a tuple
  - A field is a column is an attribute

2. What are keys in a relation?

  - Keys are one or more attribute in a relation used to identify a record, keys can be unique or nonunique

3. What is a surrogate key and how is it used?

 - A surrogate key is a column made by an arbitrary assignment of a key to a row, and is used as an alternative for natural keys which can change or become obsolete, like how a social security number should be unique to every person on the planet but is not always so or can change.

4. In the following equation, Area = Length x Width, identify the determinant(s).

 - Determinants are length and width

5. If a relation has no duplicate data, how can you be sure there is always at least one primary key?

 - Because the collection of all the attributes in the relation can identify a unique row

6. Give an example of a relation.  Determine a natural key for this relation.

 - An example of a relation would be a table with first name, last name, and address.

 For question 7 - 8, Consider product *orders*.  In particular, associated with an order is: customer name (first and last), address (street, city, state, zip), phone, email, the products orders (including item, quantity, and price). 

7. Create a relational data model for *orders*.  Consider applying normalization rules (discuss Monday)

  -

8. For customer, could email be used as a primary key?  If so, state why.  Also, if possible to use as a primary key, discuss any disadvantages of using email as a primary key.

  -

9. Given two relations S and R below find the Cartsian Product S x R. 

  -

10. Find the natural join between the Faculty and Department relations below.

  -

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
