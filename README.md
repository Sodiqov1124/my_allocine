# my_allocine
to get info from some database created this
This project will tackle one of the main tool to work with Data. You've probably heard of this tool: SQL.

SQL (Structured Query Language) is a standardized programming language that's used to manage relational databases and perform various operations on the data in them. Initially created in the 1970s, SQL is regularly used not only by database administrators, but also by developers writing data integration scripts and data analysts looking to set up and run analytical queries.

The uses of SQL include modifying database table and index structures; adding, updating and deleting rows of data; and retrieving subsets of information from within a database for transaction processing and analytics applications. Queries and other SQL operations take the form of commands written as statements -- commonly used SQL statements include select, add, insert, update, delete, create, alter and truncate.

SQL became the de facto standard programming language for relational databases after they emerged in the late 1970s and early 1980s. Also known as SQL databases, relational systems comprise a set of tables containing data in rows and columns. Each column in a table corresponds to a category of data -- for example, customer name or address -- while each row contains a data value for the intersecting column.

The sample database represents some of the data storage and retrieval about a movie related industry. Most of the people loves to watch movie, and for all of them we are providing a sample information about the movie related questions coming to their mind. This design of database will make it easier to the movie lovers to know the curiosities about the movies.

In this project, you will have to work with a database containing multiple tables. Here a description of all the tables:

Description of tables:

actors:
id – this is a unique ID for each actor
act_fname – this is the first name of each actor
act_lname – this is the last name of each actor
act_gender – this is the gender of each actor

genres:
id – this is a unique ID for each genres
gen_title – this is the description of the genres

directors:
id – this is a unique ID for each director
dir_fname – this is the first name of the director
dir_lname – this is the last name of the director

movies:
id – this is the unique ID for each movie
mov_title – this column represents the name of the movie
mov_year – this is the year of making the movie
mov_time – duration of the movie i.e. how long it was running
mov_lang – the language in which movie was casted
mov_dt_rel – this is the release date of the movie
mov_rel_country – this is the name of the country(s) where the movie was released

movies_genres:
mov_id – this is the ID of the movie, which is referencing the mov_id column of the table movies
gen_id – this is the ID of each genres, which is referencing the gen_id column of the table genres

directors_movies:
dir_id – this is the ID for each director, which is referencing the dir_id column of the table directors
mov_id – this is the ID of the movie, which is referencing the mov_id column of the table movies

reviews:
id – this is the unique ID for each reviewer
rev_name – this is the name of the reviewer

movies_ratings_reviews:
mov_id –this is the ID of the movie, which is referencing the mov_id column of the table movies
rev_id – this is the ID of the reviewer, which is referencing the rev_id column of the table reviews
rev_stars – this is indicates how many stars a reviewer rated for a review of a movie
num_o_rating – this indicates how many ratings a movie achieved

movies_actors:
act_id – this is ID of actor, which is referencing the act_id column of actors table
mov_id – this is the ID of the movie, which is referencing the mov_id column of the table movies
role – this is the name of a character in the movie, an actor acted for that character
