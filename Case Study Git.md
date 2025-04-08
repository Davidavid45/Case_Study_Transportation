**Case Study to Re-Familiarize with Transportation Data & Git-Version Control**

**Proposal :** This project aims to analyze New York City Taxi Trip data to uncover traffic patterns and commuting trends across the city. By investigating taxi trip records, the project will address key questions such as: What are the peak hours for taxi activity? How do average trip durations vary by time of day and day of the week? Which routes or boroughs experience the most congestion? Additionally, it will explore potential correlations between taxi activity and external factors (e.g., weather, special events). The overall goal is to derive actionable insights through data cleaning, exploratory analysis, and visualizations while leveraging Git for version control in VS Code.

Steps I am taking include :

**Data Acquisition** : used yellow\_tripdata\_2023-01.parquet

**Data Cleaning & Preparation**: Inspected the data, renamed the columns to fit better, removed trips above the 99th percentile to reduce skew and dropped negative durations because they’re invalid.

**Exploratory Data Analysis (EDA):** viewed the distribution of trip duration, correlation between duration, distance, distance, fare\_amount, and avg speed.

**Key findings include:** The histogram of trip durations shows that most trips are relatively short, with the majority lasting less than 20 minutes. There are fewer trips with longer durations, and extreme outliers have been removed.

There is a strong positive correlation between distance(Miles) and fare\_amount(0.93), indicating that longer trips generally cost more. duration(mins) also has a strong positive correlation with both  distance(Miles) (0.80) and fare\_amount (0.83), suggesting that longer trips in terms of time are also longer in distance and more expensive.

` `avg\_speed has a weak correlation with other metrics, indicating that speed is not strongly tied to trip distance, fare, or duration.

Hourly Fare Trends: The bar plot of average fare amounts by pickup hour reveals that fares are generally higher during late-night and early-morning hours (e.g., 11 PM to 2 AM), likely due to increased demand or longer trips during these times.

**Version Control with Git:** I initialized a local repository in VS Code, then push it remotely

<https://github.com/Davidavid45/Case_Study_Transportation.git>


