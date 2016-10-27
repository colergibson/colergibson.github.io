---
layout: post
title: Assignment 3
date: 2016-10-27
categories: "Projects"
author: "Cole Gibson"
---

# Abstract
My work was an assignment for my Management class this semester. It is a small 
action plan for a private library to use when they are converting from the Dewey
classification system to the Library of Congress classification. It outlines the
team structure, specific action items that take place in the one year allotment,
as well as how to evaluate the progress of the library patrons in accepting the
new classification and to better understand how to serve the community’s needs.

# How I converted
To convert the document I chose to ask for user input on which file they would 
like to format as well as  which conversion they wished to complete. I used 
`read` to get the user input. To successfully ensure that the program would run I
used a `while` loop to ensure that the file existed as well as an `until` loop 
to make sure that the user enters the formatting code that am able use. I then 
used specific `if` statements for each format to properly use each pandoc 
conversion that I needed.

# My Documents

- [Original Markdown File](https://github.com/inls161/assignment-3-colergibson/blob/master/Mid-Term-Project.md)

- [DOCX File](https://github.com/inls161/assignment-3-colergibson/blob/master/Mid-Term-Project.docx)

- [HTML File](https://github.com/inls161/assignment-3-colergibson/blob/master/Mid-Term-Project.html)

- [ODT File](https://github.com/inls161/assignment-3-colergibson/blob/master/Mid-Term-Project.odt)

- [PDF File](https://github.com/inls161/assignment-3-colergibson/blob/master/Mid-Term-Project.pdf)

- [Conversion Script](https://github.com/inls161/assignment-3-colergibson/blob/master/colergibson-convert-docs.sh)


Here is the link to my [Cloud9 Editor](https://ide.c9.io/colergibson/assignment3).

# Challenges
I had a few challenges in the script when I was trying to validate the user 
input. I was initially using a `while` loop with several `or` statements but I 
realized that one `False` would overwrite the rest of the statements and cause an 
infinite loop. When I tried the until loop it worked as intended so I can only 
assume that one `True` would allow the loop to end. I was also having issues with 
conversion to .html using local image files. I would be able to convert to each 
document format successfully but the images would not be found when I converted 
to .html. I fixed this error by switching to links for images instead of local 
files and that fixed my problem. Finally I had most of my problems with this 
assignment when trying to write a markdown table. I tried pipe tables, simple 
tables, grid tables all to no avail. Finally I switched back to trying simple 
tables and it worked exactly as it should. I’m still not 100% what I was 
entering incorrectly but I was able to successfully get my tables to be formatted.
