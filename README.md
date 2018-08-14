# log-Analysis
this repo is  for the implemenation of Log analysis project in udacity Nanodegree 
# Logs Analysis
Building an informative summary from logs is a real task that comes up very often in software engineering. 

# main functionality 
The objective of the Logs Analysis Project is to create a statistics tool that can answer some questions concerning the database provided during the course, the project should generate reports (in plain text) to answer the following questions 
(1) What are the most popular three articles of all time? Which articles have been accessed the most?
(2) Who are the most popular article authors of all time? 
(3) On which days did more than 1% of requests lead to errors?

 This reporting tool is a Python program using the psycopg2 module to connect to the database.




# Running the Reporting Tool

After following the instructions for installing vagrant and the database , Open the terminal. Then, run the following commands:

```
# Launch & Login to machine
cd /path/to/vagrant
vagrant up
vagrant ssh

# Open shared folder
cd /vagrant 

# Run the program
python reportgenerator.py
```

# Project output 

The reporting tool will answer the following questions

**(1) What are the most popular three articles of all time? Which articles have been accessed the most? Present this information as a sorted list with the most popular article at the top.**

Example:

Candidate is jerk, alleges rival - 338647 views
Bears love berries, alleges bear - 253801 views
Bad things gone, say good people - 170098 views

**(2) Who are the most popular article authors of all time? That is, when you sum up all of the articles each author has written, which authors get the most page views? Present this as a sorted list with the most popular author at the top.***

Example:

Ursula La Multa - 507594 views
Rudolf von Treppenwitz - 423457 views
Anonymous Contributor - 170098 views
Markoff Chaney - 84557 views



**(3) On which days did more than 1% of requests lead to errors? The log table includes a column status that indicates the HTTP status code that the news site sent to the user's browser.**

Example:

July      17, 2016 -  2.26% errors


