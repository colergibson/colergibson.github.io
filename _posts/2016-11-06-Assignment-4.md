---
layout: post
title: Assignment 4 Reflection
date: 2016-11-06
categories: ""
author: "Cole Gibson"
---
# Creating the script
When creating the script we used the notes from class to create the read input 
questions and save them to a variable. When making the .csv file we first echoed
each answer to and piped it to an .list file. We used `>>` pipes to append to the 
list instead of overwriting it. Finally we used the `paste -d, -s` command to pipe
the .list to the .csv file. The hardest part was trying to create the timestamp 
and  the Unique ID number. I was able to find the commands by searching google 
for “timestamp in bash” and “Random string in bash” Both searches were 
succesfully and I was able to modify the code to include the date and time for 
the timestamp as well as reducing the string from 32 characters to 16.

# Making the script more concise
When we finished the script I created a new branch and worked on modifying the 
script to both include user input as well as make the script more concise by 
removing the creation of the .list file. I first created a `read` statement to ask
the user which .csv file they would like to use. I then used two different `if` 
statements to see if the file already exists. I realized after I created the two
different statements I could have used an `else` statement instead of the second 
`if` statement as they would achieve the same result but I did not modify the 
script the reflect this new understanding. If the file already existed I then 
used another `read` input to ask if the user if they would like to overwrite or 
append the existing file. To make sure that the user entered what I wanted to I 
used an `until` loop to make sure that the user entered either “overwrite” or 
“append” and wouldn’t except another answer. Finally I included the same data 
entry from the original script but instead of passing it into a list I instead 
echoed each variable separated a comma directly into the .csv file.

# Links

* [Github Repository](https://github.com/gavvy/blackngreen-assignment4)
* [Concise Script Branch](https://github.com/gavvy/blackngreen-assignment4/tree/script-testing)
* [Concise Script](https://github.com/gavvy/blackngreen-assignment4/blob/script-testing/concise_script.sh)
