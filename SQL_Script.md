# Data-Driven-Decision-Making-in-SQL
SELECT a.gender, -- Report for male and female actors from the USA 
       max(a.year_of_birth), -- The year of birth of the oldest actor
       min(a.year_of_birth) -- The year of birth of the youngest actor
FROM
   (SELECT *
   From actors
   where nationality = 'USA'
   ) as a 					-- Use a subsequen SELECT to get all information about actors from the US
GROUP BY a.gender;
![Age](https://user-images.githubusercontent.com/121814714/210355930-22d67f72-e629-4dad-ace1-be8937b17b31.png)
