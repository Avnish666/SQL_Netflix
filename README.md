# Netflix Data Analysis using SQL

## 📌 Project Overview
This project analyzes Netflix’s dataset using SQL to uncover meaningful insights about its content library.  
The analysis covers content types, popular genres, top directors, and trends over time.

## 📂 Dataset
The dataset contains information about Netflix titles, including:
- **Title** – Name of the movie or show
- **Type** – Movie or TV Show
- **Director** – Name(s) of the director(s)
- **Cast** – Main actors
- **Country** – Country of production
- **Date Added** – Date added to Netflix
- **Release Year** – Year of release
- **Rating** – Audience rating (e.g., PG, R)
- **Duration** – Length in minutes or number of seasons
- **Listed In** – Genre(s)
- **Description** – Short description of the title

> Source: [Netflix Dataset on Kaggle](https://www.kaggle.com/shivamb/netflix-shows)

## 🎯 Objectives
- Identify the distribution of content by **type** (Movies vs TV Shows).
- Find the most common **genres** on Netflix.
- Discover the **top directors** by number of titles.
- Analyze content addition **trends over the years**.
- Explore content distribution by **country**.

## 🛠 Tools & Technologies
- **SQL** – Data cleaning, querying, and analysis
- **MySQL / PostgreSQL** – Database management
- **Kaggle** – Dataset source

## 📊 Key Insights
Some example findings from the analysis:
- Movies make up the majority of Netflix content.
- Drama and International Movies are among the most common genres.
- Certain directors dominate in terms of number of productions.
- Netflix’s content library has grown significantly since 2015.

## 📜 SQL Queries
Example query to count Movies vs TV Shows:
```sql
SELECT type, COUNT(*) AS total
FROM netflix
GROUP BY type;
