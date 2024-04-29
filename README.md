[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/234bMY4A)


The architechture of our system:

![GitHub Logo](image.png)
We are getting the data from Faker library. We are taking fake weather and random temperature in the range 10-110 degrees.

Then we are sending the data to apache kafka and then it is going to Apache Flink where we are processing it.

We are holding the data for 1 minute and then we are calculating the average temperature of the cities (if they are getting repeated) and then storing it in a table in postgres.

All the frameworks and postgres are used from docker after creating images.
