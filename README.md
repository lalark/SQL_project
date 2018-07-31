# SQL_project

This is my project to showcase my SQL skills. I used an Air BnB dataset that was found on Kaggle: https://www.kaggle.com/airbnb/seattle. 

I had to alter this dataset slightly in order to upload it, including: 
1. Modified  the listings.csv file to relace "" with nothing for NULLs; 
2. Fixed one line where there was a carriage return that split a number value. There are lines where there is a carriage return in the some of the text values but that seems to not cause a problem for the create and load script so I left those. It means there will be carriage returns in the values of some of the columns in the listings table in your database but presumably that will not cause a problem.

With my loaded dataset, I deduced the following:
* Identified each review as positive, negative, or neutral
* Added listing information to every review
* Grouping the reviews for each listing by quality using a left join with new quality of reviews table
* Deduced which houses in Queen Anne were available on Christmas in 2016, and had a "superhost"
* Compared the average rating of each listing to the average rating of all listings (margin of error)
* Showed all of the rental days that occurred in even months of 2016
