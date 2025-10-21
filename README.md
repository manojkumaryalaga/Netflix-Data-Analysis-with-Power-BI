## 🎬 Netflix / Movies Analysis Project
---
### 📖 Project Overview

This project analyzes a dataset of movies and to uncover insights about ratings, popularity, genres, languages, countries, directors, and cast.

Goals:

1.Identify trends in global content production

2.Find popular genres, directors, and languages

3.Explore the relationship between ratings and popularity

4.Provide actionable insights for content creators, distributors, and viewers
---
## 📊 Dataset

[Netflix Movies & TV Shows (till 2025) dataset on Kaggle](https://www.kaggle.com/code/sonawanelalitsunil/netflix-movies-tv-shows-till-2025/input?select=netflix_tv_shows_detailed_up_to_2025.csv)

Rows: 1M+ 

Columns include:
- showId – Unique identifier for each title  
- title – Name of the movie or TV show  
- director – Director(s) of the title  
- cast – List of main cast members  
- country – Country of production  
- genres – Genre(s) of the title  
- language – Language of the title  
- rating – Viewer rating  
- popularity – Popularity score  

---

### 🔧 Data Cleaning & Preprocessing

**Handling Multi-value Columns**  
- Columns such as cast, director, and country often contained multiple values separated by commas.  
- These were **split into individual entries** to enable detailed analysis by actor, director, and country.  

**Language Standardization**  
- The language column had symbols and inconsistent names.  
- A **mapping table** was used to convert abbreviations into full language names (e.g., `EN → English`, `FR → French`).  

**Removing Irrelevant Columns**  
- Removed columns that did not contribute meaningful insights to simplify analysis.  

**General Cleaning**  
- Handled missing/null values  
- Trimmed extra spaces and standardized text formatting  
- Unified categorical naming conventions  
---
### Data Cleaning Workflow Screenshots 
---
![](screenshots/Screenshot%20%2864%29.png)
---
![](screenshots/Screenshot%20%2866%29.png)
---
![](screenshots/Screenshot%20%2867%29.png)
---
![](screenshots/Screenshot%20%2868%29.png)
---
![](screenshots/Screenshot%20%2874%29.png)
---
![](screenshots/Screenshot%20%2875%29.png)
---
![](screenshots/Screenshot%20%2882%29.png)
---
### 🧮 DAX Queries

DAX measures were created to handle post-cleaning duplicates and enable meaningful aggregations:

- Distinct Movie Count – Counts each unique movie title once.

- Total Budget (Distinct) – Calculates the sum of unique movie budgets.

- Total Revenue (Distinct) – Aggregates distinct revenues per movie to avoid duplication after splitting multi-value columns.

- Language Category – Categorizes titles into English vs Non-English for comparative analysis.
---
### Screenshots
---
![](screenshots/Screenshot%20%28104%29.png)
---
![](screenshots/Screenshot%20%28105%29.png)
---
![](screenshots/Screenshot%20%28106%29.png)
---
### Netflix Dashboard 
---
![](screenshots/Screenshot%20%2892%29.png)
---
### 🔢 Key Metrics
Metric	Value	Description
- Total Screening Countries	82	Netflix movies have been released across 82 countries worldwide.
- Languages	42	Content is available in 42 different languages, showcasing Netflix’s multilingual diversity.
- Total Budget ($)	118 billion USD	The combined budget invested in movie production.
- Total Revenue ($)	346 billion USD	The cumulative revenue generated from these movies.
- Total Movies	2,975	Number of Netflix movies analyzed in the dataset.
- Genre Categories	19	Total distinct movie genres identified.

### 🌍 Geographical Insights

USA, UK, South Korea, Czech Republic, and Slovakia are the Top 5 countries by movie ratings.

The USA dominates Netflix’s production and revenue contribution.

The world map visualization indicates global content distribution, with strong activity in North America, Europe, and Asia.

### 🎭 Genre Analysis

Top Genres by Total Revenue:

Adventure

Comedy

Science Fiction

Action

Fantasy

These genres collectively contribute the highest box office revenues.

### 🌐 Language Category Breakdown

English Movies: 75.21% of total releases.

Non-English Movies: 24.79%, reflecting Netflix’s growing investment in regional and international productions.

### 🎬 Director Insights

The Top 5 Directors by Movie Count show strong correlations between budget and box office performance.

Notable directors include Ridley Scott, Guy Ritchie, Jon M. Chu, Clint Eastwood, and Steven Soderbergh, who have maintained consistent contributions to Netflix’s cinematic portfolio.
---
### ✅ Conclusion

The analysis demonstrates that Netflix maintains global dominance by:

Producing a diverse multilingual library.

Prioritizing high-budget genres like Adventure and Comedy that drive substantial revenue.

Leveraging renowned directors to maximize return on investment.

Expanding non-English productions, showing strategic regional market growth.

In summary, Netflix’s strategic mix of genre diversity, language inclusivity, and global distribution has fueled its $346B total revenue and cemented its position as a leader in global entertainment streaming.
