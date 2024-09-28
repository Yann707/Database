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
![11](https://github.com/user-attachments/assets/69954301-a635-4f77-8122-274b4511db7b)
#2 select airports.name as 'airports name' from airports, country where airports.iso_country = country.iso_country and country.name = 'France' and airports.type = 'large_airport';
![12](https://github.com/user-attachments/assets/6354eb3f-fdbe-476e-8a8d-89686f47c6aa)
#3
![13](https://github.com/user-attachments/assets/65ebc630-2aac-443d-b7c5-c925f74d1b0c)
#4
![14](https://github.com/user-attachments/assets/720efe0c-71fc-4883-b6b5-e05c47d49e67)
#5
![15](https://github.com/user-attachments/assets/739441ed-863a-4db0-824b-c2efd5b0c9d3)
#6
![16](https://github.com/user-attachments/assets/74eb42f6-a963-423a-bc05-4a91d1ad8b6d)
#7
![17](https://github.com/user-attachments/assets/9b1c59a7-224a-4f6f-bf68-78debbe01db7)
#8
![18](https://github.com/user-attachments/assets/d5bdfad3-fdbf-45ab-ad8b-0b79ee740d95)
#9
![19](https://github.com/user-attachments/assets/d63985c0-1827-4408-bc2e-e7e26e7b2f52)
#10
![20](https://github.com/user-attachments/assets/3a36de3d-4ebe-456b-90e0-f941fcdb7082)










