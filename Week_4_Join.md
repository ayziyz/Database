# Week 4

### Assignment: Join

### Question 1
Select country.name as "country name", airport.name as "airport name" 
from country join airport on country.id = airport.id where country.name = "Finland";

![screenshot](/Screenshots/Join_1.png)

### Question 2
select screen_name, airport.name from game inner join airport on location = ident;

![screenshot](/Screenshots/Join_2.png)

### Question 3
select screen_name, country.name from game inner join airport on location = ident;
inner join country on airport.iso_country = country.iso_country;

![screenshot](/Screenshots/Join_3.png)

### Question 4
select airport.name, screen_name from airport left join game on ident = location where airport.name = "%Hels%";

![screenshot](/Screenshots/Join_4.png)

### Question 5
select name, screen_name from goal left join goal_reached on goal.id = goal_id left join game on game.id = game_id;
![screenshot](/Screenshots/Join_5.png)