# Disneyland-Reviews

## Project Objective

This project analyzes reviews of three Disneyland parks (Disneyland Hong Kong, Disneyland Paris, and Disneyland California) over several decades. Using Tableau for visualization and data analytics, we will explore sentiment analysis of the reviews, identify trends over time, and assess ratings for each park to uncover the key factors influencing these ratings.

## Objectives

The primary objectives of this project are:

1. Explore Customer Preferences:
    - Identify which park has the highest number of reviews and which has the highest ratings
    - Analyze the percentage distribution of star ratings for each park and the distribution of parks based on star ratings
2. Examine Review Locations:
    - Explore the geographic distribution of reviews
    - Determine average star rating per location
3. Identify Temporal Trends:
    - Conduct a time analysis to identify patterns in ratings throughout the year and across different months.
4. Provide Data-Driven Insights:
    - Generate insights to optimize Disneyland’s performance based on customer reviews.
  
## Data Preprocessing 

The dataset was cleaned to address missing values in the Month and Year columns. Rather than dropping these rows, word matching was employed to extract the month and year from the Review column where applicable, maximizing the dataset's value.

Sentiment analysis was conducted on the reviews using Natural Language Processing techniques. This analysis identified the most frequent words associated with high scores (>0.5) and low scores (<0.5).

## Tableau Visualizations

The project includes a series of interactive Tableau dashboards covering:

- **Percent Distribution of Star Rating Per Park:** Bar charts illustrating the proportion of star ratings across each park.
- **Percent Distribution of Park Per Star Rating:** Pie chart configurable by a filter of 1-5 Star Rating, showcasing the proportion of each park corresponding to each star rating.
- **Average and Number of Reviews by Location:** Bar charts displaying average ratings and total review counts for various locations.
- **Most Common Words Associated with High and Low Sentiment Scores:** Bar chart displaying Top 10 frequent terms linked to high and low sentiment ratings.
- **Rating Over the Year and Month: **Line charts depicting trends in ratings over time, broken down by month and year.

Visit the [Tableau Dashboard](https://public.tableau.com/app/profile/melody.feng/viz/Disneyland_Reviews_Visualization/StarRatingDistribution) to explore the visualizations and insights.


## Key Questions and Insights

### 1. Which Disneyland park is the most popular among visitors, and how does visitor satisfaction compare across parks?

Analysis: I explored how star ratings are distributed among the parks, as well as the average ratings and total review counts based on reviewer location.

Visualization: Percent Distribution of Star Rating Per Park (Bar Chart), Percent Distribution of Park Per Star Rating (Pie Chart), Average and Number of Reviews by Location (Bar Chart).

Insight: Disneyland California has the highest number of reviews among all Disneyland parks having also the most  reviews from the USA, with 63.83% of those reviews being 5 stars. Additionally, 53.87% of all 5-star ratings across all Disneyland parks are for Disneyland California, highlighting its popularity and appeal.

<img width="980" alt="Screenshot 2024-10-18 at 11 38 54 PM" src="https://github.com/user-attachments/assets/219c3ddc-ad05-445d-bee3-4eb3f719a571">

### 2. What factors influence the ratings and sentiment of visitors to the park?

Analysis: I identified the most common terms associated with high and low sentiment ratings.

Visualization: Bar chart displaying Top 10 frequent terms linked to high and low sentiment ratings.

Insight: Words about rides, wait and time show up in both high and low sentiment reviews, suggesting that the ease of getting on rides significantly influences ratings. Those with higher sentiment likely experienced shorter wait times, possibly due to having passes.

<img width="976" alt="Screenshot 2024-10-18 at 11 27 33 PM" src="https://github.com/user-attachments/assets/ad183a8a-759d-44d2-b2b0-b84faa49b5cf">

### 3. Is there a trend in star ratings over the years?

Analysis: I evaluated the trends in average star ratings across the years.

Visualization: Line chart displaying average star ratings over the years for each park.

Insight: Overall, the parks experienced their lowest ratings in the year 2006 with a stable trend from 2008 onwards to 2019. 

<img width="1431" alt="Screenshot 2024-10-19 at 12 07 59 AM" src="https://github.com/user-attachments/assets/f75b9231-6132-4dc1-bcde-c3fea528c745">

### 4. Is there a trend in star ratings over the months?

Analysis: I analyzed the trends in average star ratings by month, aggregated over the years.

Visualization: Line chart showing average star ratings for each park across the months.

Insight: Parks generally saw the lowest ratings in August and the highest in September, potentially due to factors like longer wait times during summer vacations in August and reduced crowds as school resumes in September.

<img width="1321" alt="Screenshot 2024-10-19 at 12 07 27 AM" src="https://github.com/user-attachments/assets/f3a6b305-8665-44d8-9eaf-b7345eeef121">

### Note: 
_I analyzed star ratings by month and year without filtering by park as this provides holistic insights into overarching trends and visitor behavior that affect all parks collectively. This approach helps identify external factors, such as holidays or events, that may influence visitor satisfaction across multiple locations, while minimizing individual biases that could skew results for each park, enabling better strategic planning and operational adjustments._

## Conclusion and Recomendations 

Based on the insights from this analysis

**1. Enhance Ride Efficiency:** Increase resources and strategies aimed at reducing wait times and improving ride accessibility to boost visitor satisfaction.

**2. Monitor Seasonal Trends:** Adjust staffing and operational strategies during peak months, particularly August, to better manage visitor flow and enhance experiences.

**3. Investigate Historical Context:** Conduct an analysis of factors contributing to the low ratings in 2006 to implement learnings and prevent future declines.

**4. Leverage High Satisfaction Insights:** Use the success of Disneyland California as a model to identify best practices that can be implemented across other parks to enhance overall guest experiences.

**5. Tailor Marketing Strategies by Reviewer Location:** Analyze the demographics and preferences of reviewers based on location to create targeted marketing campaigns that attract visitors from specific regions, enhancing park appeal and attendance.

## Dataset

The dataset used in this analysis comprises 42,000 reviews from three Disneyland locations: Paris, California, and Hong Kong, submitted by visitors on TripAdvisor.

### Key Attributes:

- **Location Data:** Disneyland branch, reviewer location, country of origin
- **Review Data:** Review ID, rating, year and month of visit, review text
- **Visitor Data:** Visitor demographics, including reviewer location and country of origin
- **Sentiment Data:** Sentiment scores derived from review text, common terms used

This project uses Disneyland data sourced from [Kaggle](https://www.kaggle.com/datasets/arushchillar/disneyland-reviews/data).
