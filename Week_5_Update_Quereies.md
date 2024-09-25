# Week 4

### Assignment: Subqueries

### Question 1
update game
set  location = (select ident from airport where name = "Nottingham Airport"), co2_consumed = co2_consumed+500
where screen_name = "Vesa";

select * from game;
![screenshot](/Screenshots/Update_1.png)

### Question 2
Goal_reached

### Question 3
DELETE FROM goal_reached; 

Select * from goal_reached;
![screenshot](/Screenshots/Update_2.png)

### Question 4
Delete from game;

Select * from game;
![screenshot](/Screenshots/Update_3.png)

