## 🎬 Netflix / Movies Analysis Project
### 📖 Project Overview

This project analyzes a dataset of movies and to uncover insights about ratings, popularity, genres, languages, countries, directors, and cast.

Goals:

1.Identify trends in global content production

2.Find popular genres, directors, and languages

3.Explore the relationship between ratings and popularity

4.Provide actionable insights for content creators, distributors, and viewers

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

### 🧮 DAX Queries

DAX measures were created to handle post-cleaning duplicates and enable meaningful aggregations:

Distinct Movie Count – Counts each unique movie title once.

Total Budget (Distinct) – Calculates the sum of unique movie budgets.

Total Revenue (Distinct) – Aggregates distinct revenues per movie to avoid duplication after splitting multi-value columns.

Language Category – Categorizes titles into English vs Non-English for comparative analysis.
