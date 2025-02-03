# tableau-challenge

Analysis is written in a markdown file or included in the Tableau Public workbook (5 points)
Analysis describes the dashboards and any interesting data discoveries contained within them (5 points)
Analysis on the chosen city official requested map detailing any noticeable trends (5 points)
The written analysis references specific visualizations and interactive features (5 points)
The document is written in a manner that a non-technical reader could understand (5 points)

## Background

Per Bootcamp Spot Website:
>
> Congratulations on your new job! As the new lead analyst for the New York Citi BikeLinks to an external site. program, you are now responsible for overseeing the largest bike-sharing program in the United States. In your new role, you will be > expected to generate regular reports for city officials looking to publicize and improve the city program.
> 
> Since 2013, the Citi Bike program has implemented a robust infrastructure for collecting data on the program's utilization. Each month, bike data is collected, organized, and made public on the Citi Bike DataLinks to an external site. webpage.
> 
> However, while the data has been regularly updated, the team has yet to implement a dashboard or sophisticated reporting process. City officials have questions about the program, so your first task on the job is to build a set of data reports to provide the answers.


## Assignment Breakdown

1. Download zip files from the CitiBike NYC website for [trip data](https://s3.amazonaws.com/tripdata/index.html).
2. For this assignment, I chose to focus on the last 3 months of 2024. The zip files are rather large in size and contain millions of rows of data.
3. I loaded the CSV files from the zip files into a Jupyter Notebook and used the pandas Python library to take a quick look at the data and also clean it (removing null value rows, for example).
4. After cleaning, I exported the new CSV files to load into Tableau and began my exploratory analysis.

## Analysis


### Number of Rides

I first aimed to get the number of CitiBike rides for my chosen date range (Oct 2024 - Dec 2024). Member riders comprised the large majority of bike rentals vs Casual riders -- 9.24 million vs 1.88 million, respectively.

It became immediately obvious that the number of bike rentals dropped significantly as the months progressed and the season changed from autumn to winter.

The number of rides remained steady through the month of October but declined in November, with a sharp drop on the 21st of the month. In total, there were 1,436,021 less rides in November from October.

The decline continued in December, with 1,393,567 less rides than November. The sharp decline can be attributed to colder temperatures as the season transitioned from autumn to winter. The average temperature in October was in the 60 degree (Fahrenheit) range. By December, the average temperature was in the 30s-40s.

There appeared to be a Holiday effect, too. There were far less rides on Thanksgiving Day, 11/28 -- the smallest number of rides for the entirety of November. 

December saw the least amount of rides on the days leading up to and including Christmas (the 21st, 22nd, 24th, and 25th).
