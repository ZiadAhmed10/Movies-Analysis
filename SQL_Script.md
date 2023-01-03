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
![Age](https://user-images.githubusercontent.com/121814714/210357296-ad5679a3-f700-4353-a1d1-00e1eaa332cc.png)

