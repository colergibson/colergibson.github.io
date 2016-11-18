---
layout: post
title: Assignment 5 Reflection
date: 2016-11-17
categories: ""
author: "Cole Gibson"
---
# Creating Our Scripts
We had three different scripts that we used to create and populate the database.
The first script is to create the database as well as to create the table with 
each of the fields set to varchar 255. We also load in the data from the csv 
file. The last thing in the script is to create a new user with a password so 
that an individual would not have to rely on using their own personal username 
and password to work with the database. The next script was the one that was 
used to prompt the user for the data and then enter it into the database. Before
we asked the user for the data though we checked to see if there was an initial 
dump file so that the user will have an up to date table. We also used a smaller
script to load in the changes to the csv file that reflected the new data that 
was inputted. After we collected the data we then asked the user if they wanted 
to import the data into the table as well as asking if they would like to export
the file by creating a dump file.

# Personal Challenges
I was responsible for creating the initial scripts and re-coding the data input 
script to pass the data into the table. My main challenges were in creating the 
csv file after the new data was entered. When I first wrote the script it would 
enter the data on the same line as the last entry in the csv file the first time
but the second time the script was run the data was entered on a new line. The 
script was indented in an if statement when this was happening and when I 
removed the if statement and the indention’s it ran properly. The only other 
challenge was getting the data to be entered without duplicate entries. I was 
having problems when I was first running the program as I wasn’t using a dump 
file and was just running the script as if I was the first person using it. I 
also was appending to the csv file so that when I loaded the data into the table
it would have multiple entries. I was able to resolve this by including a 
conditional statement to see if the dump file existed for future users and then 
I changed the csv file to be overwritten instead of appended so that the data 
would not be entered multiple times.

# Links

* [Github Repository](https://github.com/jamiemramos/blackngreen)
