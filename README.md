# Work-Simulation-2-project
A Simulation program at MITT
Instructions
You are given the following 3 text files:

Movies.txt: represents a set of movies. Each line represents a single movie, the line is divided by a pipe character ( ‘|’), in this file we only care about the first two columns in each line, the first column is the movie Id, the second is the movie Name, the rest of the line is not important.

Users.txt: represent a set of users, each line represents a single user, the line is divided by a pipe character ( ‘|’), for example, here is the first line in the file:

1|24|M|technician|85711

The columns represent the user id, age of the user, gender, occupation. The last column is not important for us.

Ratings.txt: represent a set of ratings from users on movies, each line represents a single rating from a user on a movie, the line is divided by the tab character, for example, here is the first line:

196    242    3    881250949

The first number is the user id, then the movie Id, then the rating (ratings are numbers 

1 to 5), The last column is not important for us.


Your job is to:

Create a new database with three tables: Movie, User and Rating (Note that the Id should not be auto incremented, you need to read it from the file).

Write 3 Stored procedures to INSERT a new Movie, User, and Rating. Each should be provided the proper set of parameters so that they can insert table items programmatically.

Create a C# console application, this application will have the following functions in this order:

InsertUsers: This function will read the lines from the file Users.txt and call the stored procedure for each line to insert a new user in the User table.

InsertMovies: This function will read the lines from the file Movies.txt and call the stored procedure for each line to insert a new movie in the Movie table.

InsertRatings: This function will read the lines from the file Ratings.txt and call the stored procedure for each line to insert a new rating in the Rating table.

Your application should reach each item in each file. The result should be a full database. You should review your new database to make sure that it is free of errors.

Write the following stored procedures, then call them in the C# application:

All The Movies Rated by a User

Average rating for a movie

Average rating for all movies (for each movie)

Top average rated movie

Top 10-average-rated Movies

Worst Movie (The movie with lowest average rating)

Bonus Question:

In the Movies.txt file, the third column in each line is the date the movie was released. Write a new stored procedure to UPDATE all movies to include their date from the file, then write a new function in the console application to UPDATE all movies using this stored procedure.

Submit a .zip file containing:

C# Code

A .txt file of your stored procedures

3 screenshots of the data in the tables. The output of a simple SELECT statement will do.
