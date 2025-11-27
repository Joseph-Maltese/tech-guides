# What determines which table is left or right in a SQL join?
Here is the key rule: the table that appears first (right after the FROM clause) will be designated as the LEFT table, unless the join is a RIGHT join; in which case the table order is reversed. These are the only determining factors; the order of tables in the ON clause has nothing to do which table is LEFT or RIGHT.

Let's reinforce our understanding with some examples.

FROM A INNER JOIN B ON … (left table is A)

FROM A LEFT JOIN B ON … (left table is A)

FROM A RIGHT JOIN B ON … (left table is B)

FROM A FULL JOIN B ON … (left table is A)

FROM A JOIN B ON B.id = A.id (left table is A)
<br>
<br>
That's it! Thanks for reading and keep practicing.









