# Week 3

### Assignment: Multiple Table Queries

### Question 1
select country.name as "country name", airport.name as "airport name"  from country, airport 
where airport.iso_country = country.iso_country and country.name = "Iceland";

![screenshot](/Screenshots/MultipleTable_1.png)

### Question 2
select airport.name as "Airport Name" from airport,country 
where airport.iso_country = country.iso_country and country.name = "France" and airport.type = "large_airport"; 
![screenshot](/Screenshots/MultipleTable_2.png)

### Question 3
Select country.name as "country_name", airport.name as "airport_name" from airport,country 
where airport.iso_country = country.iso_country and country.continent = "AN";
![screenshot](/Screenshots/MultipleTable_3.png)

### Question 4
select elevation_ft from airport,game where game.location = ident and screen_name ="Heini";
![screenshot](/Screenshots/MultipleTable_4.png)

### Question 5
select elevation_ft * 0.3048 as "elevation_m" from airport,game where game.location = ident and screen_name ="Heini";
![screenshot](/Screenshots/MultipleTable_5.png)

### Question 6
select name from airport,game where location = ident and screen_name = "Ilkka";
![screenshot](/Screenshots/MultipleTable_6.png)


### Question 7
select country.name from airport,country,game 
where airport.iso_country = country.iso_country and location = ident and screen_name = "Ilkka";
![screenshot](/Screenshots/MultipleTable_7.png)

### Question 8 
select name from goal, goal_reached, game  where game_id and goal.id = goal_id and screen_name = "Heini";
![screenshot](/Screenshots/MultipleTable_8.png)

### Question 9
select airport.name from game, goal_reached, goal, airport 
where ident = location and game.id = game_id and goal.id = goal_id and screen_name = "Ilkka" and goal.name = "CLOUDS";
![screenshot](/Screenshots/MultipleTable_9.png)

### Question 10
select country.name from game, goal_reached, goal, country, airport 
where airport.iso_country = country.iso_country and ident = location and game.id = game_id and goal.id = goal_id and screen_name = "Ilkka" and goal.name = "CLOUDS";
![screenshot](/Screenshots/MultipleTable_10.png)