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
#  Exercise 3  
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
# Exercise 4 
#1 select country.name as "country name", airports.name as "airports name" 
from country inner join airports on airports.iso_country = country.iso_country 
where country.name = "Finland" and scheduled_service = "yes";
![21](https://github.com/user-attachments/assets/cd4109c3-2f1e-4c9d-96a5-428e8c652ad9)
#2 select screen_name, name from game inner join airports on airports.ident = game.location;
![22](https://github.com/user-attachments/assets/6681be04-e24c-4287-989e-5d02140fb15b)
#3 select country.name as country_name, airports.name as airports_name 
from country, airports
where airports.iso_country = country.iso_country and country.continent = 'AN';
![23](https://github.com/user-attachments/assets/e93f90a8-793b-4bb0-a08d-679dec3aafed)
#4 select name, screen_name from airports left join game on ident=location where name like "%Hels%";
![24](https://github.com/user-attachments/assets/85925371-2681-4a76-8290-09180adfa9e1)
#5 select name, screen_name from goal left join goal_reached on goal_id =goal.id left join game on game.id= game_id
![25](https://github.com/user-attachments/assets/47c54a65-3982-4252-a800-0c54a09e1c76)
# Exercise 5
#1 select name from country where iso_country in( select iso_country from airport where name like 'Satsuma%' ); 
<img width="497" alt="31" src="https://github.com/user-attachments/assets/0ed607bb-6192-424e-aa94-ebf163d8c5c0">
#2 select NAME 
from airports 
where iso_country in( select iso_country from country where name = 'Monaco' );
![32](https://github.com/user-attachments/assets/71172f12-ef8e-4453-bed1-6e0eeb0772e7)
#3 select screen_name from game where id in( select game_id from goal_reached where goal_id in( select id from goal where name = 'CLOUDS') );
![33](https://github.com/user-attachments/assets/66a88017-87be-4e19-8117-50e0b58f8db3)
#4 select name from country where iso_country not in( select iso_country from airports );
![34](https://github.com/user-attachments/assets/509d09d2-29fa-4951-af3b-526182e4c713)
#5 select name from goal where id not in( select goal_id from goal_reached where game_id in( select id from game where screen_name = 'Heini' ) );
![35](https://github.com/user-attachments/assets/ba8e47b3-34f4-40e9-a0e9-17d3ac4bb954)
# Exercise 6
#1 select max(elevation_ft) from airports;
![image](https://github.com/user-attachments/assets/85c46698-7ac2-4cbf-8f64-4fd5ffab5e4c)
#2 select continent, count(*) from country group by continent;
![image](https://github.com/user-attachments/assets/9e17ca5f-c955-454a-a05f-f95f79b9dff1)
#3 select screen_name, count(*) from game, goal_reached where id = game_id group by screen_name;
![image](https://github.com/user-attachments/assets/62744522-69b8-41b9-bbdd-4e7040e7eac0)
#4 select screen_name from game where co2_consumed in( select min(co2_consumed) from game );
![image](https://github.com/user-attachments/assets/f856850a-e96d-463b-bd95-4e16fe38b5d9)
#5 select country.name, count() from country, airport where country.iso_country = airport.iso_country group by country.iso_country order by count() desc limit 50;
<img width="770" alt="11" src="https://github.com/user-attachments/assets/b39bf9fe-ac98-4dfe-b756-18857c362efe">

#6 select country.name 
from airports, country 
where airports.iso_country = country.iso_country group by country.iso_country having count(*) > 1000;
![image](https://github.com/user-attachments/assets/34fe3510-9e9a-4691-94c4-3477e5bb3c17)
#7

#8

#9

#10
