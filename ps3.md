Problem Set 3

1.)Define the terms: relation, tuple, attribute, record, and field.
    Tuple and Record are synonyms for 'row' and Attribute and Field are synonyms for 'column'.

2.)What are keys in a relation?
    Keys are unique indentifiers in a regulation.

3.)What is a surrogate key and how is it used?
    A surrogate key is an auto-incremented integer with no connection to data. It is used independent of the item(s).

4.)In the following equation, Area = Length x Width, identify the determinant(s).
    Length and Width are the determinants.

5.)If a relation has no duplicate data, how can you be sure there is always at least one primary key?
    You can be sure there is always at least one primary key because the collection of all attributes in the relation can idetify a   unique row.

6.)Give an example of a relation. Determine a natural key for this relation.
    An example of a relation would be a table... A table of students that had student ID numbers, student first names, student last names, their department IDs, and their advisor's IDs.

For question 7 - 8, Consider product orders. In particular, associated with an order is: customer name (first and last), address (street, city, state, zip), phone, email, the products orders (including item, quantity, and price).

7.)Create a relational data model for orders. Consider applying normalization rules (discuss Monday)
    Table of customers
        *name_last
        *name_first
        *customer_id (PK)
        *phone
        *street address
        *city
        *state
        *zip (FK)
        *email
        
    Zip Table
        *zip (PK)
        *city
        *State
    
    Products Table
        *product_id (PK)
        *cost (cost company buys for)
        *MSRP (price company sells for)
        
    Orders Table
        *order_id (PK)
        *customer_id (FK)
        
    Order Deatils Table
        *order_detail_id (PK)
        *quantity
        
    
   
8.)For customer, could email be used as a primary key? If so, state why. Also, if possible to use as a primary key, discuss any disadvantages of using email as a primary key.
    Email would be a good primary key because it's unique to one person. The only disadvantage would be the person no longer using a certain email or a person having more than one email.

9.)Given two relations S and R below find the Cartsian Product S x R.
    A	B C	D	E
    1	2 3	1	1
    2	3 2	2	3
    0   0 2	1	5

10.)Find the natural join between the Faculty and Department relations below.
    The natural join is Department.

S

A	B
1	2
2	3
R

C	D	E
3	1	1
2	2	3
2	1	5
Faculty

Name	ID	Dept
Joe	1	Chemistry
Susan	2	Math
Tom	3	Marine Science
Mike	4	Math
Department

Dept	Chair
Chemistry	John
Math	Mike
Marine Science	Barry
