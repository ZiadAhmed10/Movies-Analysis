# Data-Driven-Decision-Making-in-SQL
SELECT a.gender,  
       max(a.year_of_birth), 
       min(a.year_of_birth) 
FROM
   (SELECT *
   From actors
   where nationality = 'USA'
   ) as a 					
GROUP BY a.gender;
![Age](https://user-images.githubusercontent.com/121814714/210355930-22d67f72-e629-4dad-ace1-be8937b17b31.png)
