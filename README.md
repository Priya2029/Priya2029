Project Objective
This project demonstrates data analysis skills using a dataset of Zomato restaurant listings. The primary goal was to practice and showcase proficiency in SQL and the Python pandas library by answering a series of analytical questions, ranging from basic data retrieval to more complex aggregations and classifications.

Dataset
The analysis was performed on the Zomato_Dataset.csv file, which contains detailed information about restaurants across multiple countries. The key columns used in this analysis include:

RestaurantName

CountryCode, City

Cuisines

Average_Cost_for_two

Price_range

Rating

Votes

Analytical Questions & Findings
Several key questions were explored to understand the dataset. Below are the summaries of the analyses and their findings.

1. Distribution of Restaurants by Price Range
Question: How many restaurants fall into each price range category?

Approach: The data was grouped by the Price_range column, and the number of restaurants in each group was counted.

Finding: The majority of restaurants in the dataset fall into the lower price ranges, with the count decreasing significantly as the price range increases.

Price Range 1: 4,444 restaurants

Price Range 2: 3,113 restaurants

Price Range 3: 1,408 restaurants

Price Range 4: 586 restaurants

2. Restaurant Classification by Cost
Question: How many restaurants are 'Budget-Friendly', 'Mid-Range', and 'Expensive'?

Approach: A new category was created for each restaurant using a CASE statement (in SQL) or a function (in pandas) based on the Average_Cost_for_two.

Budget-Friendly: Cost < 500

Mid-Range: Cost between 500 and 1500

Expensive: Cost > 1500

Finding: The dataset is heavily skewed towards budget-friendly options.

Budget-Friendly: 5,174 restaurants

Mid-Range: 3,793 restaurants

Expensive: 584 restaurants

3. Relationship Between Ratings and Votes
Question: What is the average number of votes for restaurants in different rating categories (e.g., 1-1.9, 2-2.9, etc.)?

Approach: The ratings were binned into categories. Then, the data was grouped by these new categories to calculate the average number of votes for each.

Finding: A strong positive correlation was found: higher-rated restaurants receive significantly more votes. This suggests higher customer engagement with better-quality restaurants. Interestingly, no restaurant in the dataset had a perfect 5.0 rating.

Rating Category	Average Votes
1.0 - 1.9 (or lower)	1.0
2.0 - 2.9	46.0
3.0 - 3.9	134.0
4.0 - 4.9	593.0

Export to Sheets
4. Country-Level Analysis
Question: For each country, which city has the most restaurants, and where is the highest-rated restaurant located?

Approach: The data was grouped by country to find both the city with the maximum restaurant count and the restaurant with the maximum rating within that country.

Finding: The analysis provided a global overview of the restaurant landscape. India dominates the dataset, with New Delhi having the most listings. The highest rating achieved in most countries was 4.9, highlighting the rarity of a perfect score.

Tools and Libraries
Language: Python

Library: pandas for data manipulation and analysis

Environment: Google Colab / Jupyter Notebook

Concepts: SQL (for logical query structure)
