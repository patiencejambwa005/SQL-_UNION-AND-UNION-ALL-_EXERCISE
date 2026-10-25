# SQL-_UNION-AND-UNION-ALL-_EXERCISE
This project demonstrates the difference between SQL UNION and UNION ALL using examples related to banking transactions and high risk customer watch lists

*Objectives*
*understand how UNION works
*understand how UNION ALL works
*learn when to use each SQL operator

1 UNION 
*UNION combines the results of two or more SELECT statements and removes duplicate rows

SELECT customer_id
FROM january_ watchlist
UNION
SELECT customer_id
FROM february_watchlist;

*this query returns a unique list of customers who appeared on either the January or February high-risk watch list


2 UNION ALL 
*UNION ALL combines the results of two or more results or more SELECT statements and keeps duplicate rows

SELECT transaction_id
FROM january_transactions
UNION ALL 
SELECT transaction_id
FROM february_transactions;

*this query keeps all returned transaction records,including duplicates 

#Difference Between UNION and UNION ALL# 
*UNION removes duplicate rows
*UNION ALL keeps duplicate rows 
*UNION ALL is generally faster because it does not remove duplicates

#Both SQL operators combine results from multiple SELECT statement ,UNION is useful when unique results are required,while UNION ALL is useful when every returned record must be preserved#

#Skills Practised#
*SQL SELECT statements
*combining query results
*identifying duplicate records
*apply SQL to banking examples

