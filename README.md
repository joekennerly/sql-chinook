# SQL is awesome!

This is from the NSS server-side course

https://github.com/nashville-software-school/bangazon-llc/blob/master/book-5-data/chapters/CHINOOK.md 

## Common Selections

*Concat two columns into one*
SELECT c.FirstName || ' ' || c.LastName AS "Full Name"
FROM Customer c;

*Filter entries to only show one instance of each*
SELECT DISTINCT i.BillingCountry
FROM Invoice I;

*Format date by year*
strftime( '%Y', i.InvoiceDate) AS Year

*Limit the number of decimal places*
ROUND(SUM(i.Total), 2)
