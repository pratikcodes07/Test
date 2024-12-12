Zomato Restaurant Data Analysis

Problem Statement:-

This dashboard helps the zomato understand their customers better. It helps the zomato know if their customers are satisfied with their services. Through different ratings, they get to know their improvement area, & thus they can improve their services by identifying these area. It also lets them know the average delay & departure time, thus since by using this dashboard they have identified this problem, they can further work on factors responsible for these unwanted delays.

Steps followed:-

Step 1 : Load data into Power BI Desktop, dataset is a csv file.

Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.

Step 3 : Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".

Step 4 : It was observed that in none of the columns errors & empty values were present except column named "Arrival Delay".

Step 5 : From the zomato restaurant dataset four columns were identified which were of not any use for this analysis so they were dropped,"Address","Locality","Longitude","Latitude".

Step 6 : Both the datasets were merged i.e.the restaurant dataset and the country dataset where mapping was done on the country code column.

Step 7 : In the report view, under the view tab, theme was selected.

Step 8 : Since the data contains various ratings,cities,countries and restaurants thus in order to represent these measures, a new measure for all of them was added.

Step 9 : Four Slicers were added to the canvas, representing deliverying status of the restaurant, online delivery, price and the country of the restuarants and all the slicers with the help of format were added the drill down feature.

Step 10 : A clustered bar chart was also added to the report votes by rating text, i.e. sum of votes by rating text.

Step 11 : A stacked column chart was added to represent total restaurants with the rating text.

Step 12 : A tree chart was added for the cuisines where the distribution of the cuisines is made.

Step 12 : In the report view, under the insert tab, one text boxes were added to the canvas, in company's was name(Zomato Data Analysis) was mentioned

Step 13 : In the report view, under the insert tab, using the image insert zomato comapany's Logo was inserted.

Step 14 : Calculated column was created in which, total of restaurants,country and city was calculated.

for creating new column following DAX expression was written;

  total restaurants = DISTINCTCOUNT(zomato[restaurants])
  total country = DISTINCTCOUNT(zomato[country])
  total city = DISTINCTCOUNT(zomato[city])
    
Step 15 : New measure was created to find total count of customers.

Insights:-

A single page report was created on Power BI Desktop & it was then published to Power BI Service.

Following inferences can be drawn from the dashboard;

[1] Total Number of Restaurants = 9545
[2]Max Ratings of total restaurants by cuisines
a) North Indian - 3k
b) Chinese - 2k
c) Fastfood - 1k
