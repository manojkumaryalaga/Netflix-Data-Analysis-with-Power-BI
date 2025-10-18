## 🎬 Netflix / Movies Analysis Project
### 📖 Project Overview

This project analyzes a dataset of movies and to uncover insights about ratings, popularity, genres, languages, countries, directors, and cast.

Goals:

1.Identify trends in global content production

2.Find popular genres, directors, and languages

3.Explore the relationship between ratings and popularity

4.Provide actionable insights for content creators, distributors, and viewers

## 🗂 Dataset Description

Dataset Source

This analysis utilizes the dataset from Kaggle:

Netflix Movies and TV Shows (up to 2025)

Columns

showId – Unique identifier for each title

title – Name of the movie or TV show

director – Director(s) of the title

cast – Main cast members

country – Country of production

genres – Genre(s) of the title

language – Language of the title

rating – Viewer rating

popularity – Popularity score

🔧 Data Cleaning & Preprocessing
Handling Multi-value Columns

Columns like cast, director, and country often contain multiple values separated by commas.

These were split into individual entries to allow detailed analysis of each actor, director, and country.

Language Standardization

The language column contained symbols, abbreviations, or inconsistent names.

A mapping table was created to convert all entries into standard full language names (e.g., EN → English, FR → French).

Removing Irrelevant Columns

Columns without analytical value were removed to reduce noise.

General Cleaning

Handled missing/null values

Trimmed extra spaces and standardized text formatting
