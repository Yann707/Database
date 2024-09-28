# Exercise2
#1 select* from goal;
![1](https://github.com/user-attachments/assets/846fb207-7c41-45e6-853d-8ea00148cea0)
#2 select name, type from airports where iso_country = 'FI';    
![2](https://github.com/user-attachments/assets/7a0e79ca-3fac-4888-b506-4b48ea3535f9)  
#3 select name from airports where iso_country = 'FI' order by name;    
![3](https://github.com/user-attachments/assets/98e02b8e-1735-4d82-83f2-e0ba8dfa9a66)
#4 select name, type from airports where iso_country = 'FI' order by type, name; 
![4](https://github.com/user-attachments/assets/b8bf9f05-9237-472e-a237-229709346f73)
#5 select name from country where name like 'F%';
![5](https://github.com/user-attachments/assets/1d447ec7-fae5-4eeb-89b6-b22e729fe3bc)
#6 select name from country where name like '%F%';
![6](https://github.com/user-attachments/assets/4f4a4887-6346-4ab0-a2e5-4d93ab4b5244)
#7 select location from game where screen_name = 'Vesa' ; 
![7](https://github.com/user-attachments/assets/40941112-c2f3-40f2-ba4e-00b8bc8d35b5)
#8 select co2_consumed from game where screen_name = 'Ilkka'; 
![8](https://github.com/user-attachments/assets/52dc75a1-8a2e-4c63-b804-9c04953f4647)
#9 select distinct co2_budget from game;
![9](https://github.com/user-attachments/assets/9f219dcc-6573-470a-a882-a74ed9ca868d)
#10 select screen_name, co2_budget, co2_consumed, @co2_left := (co2_budget - co2_consumed) AS co2_left FROM game WHERE screen_name = 'Ilkka';
![10](https://github.com/user-attachments/assets/21fe3d9d-4802-4374-a50e-869b95169cc4)
#Exercise 3  
#1 select country.name as "country name", airports.name as "airports name" from airports, country where airports.iso_country = country.iso_country and country.name = "Iceland";









