# Netflix Movies & TV Shows — Exploratory Data Analysis

Exploratory Data Analysis (EDA) on Netflix's public content catalog to uncover trends in genre popularity, content additions over time, and country-wise distribution of titles.

## Objective
Understand how Netflix's content library has grown and evolved — what kinds of content dominate, where it comes from, and how additions have trended over time — using Python's data analysis and visualization stack.

## Dataset
- **Source:** Netflix Movies and TV Shows dataset (originally published on Kaggle, distributed via [TidyTuesday](https://github.com/rfordatascience/tidytuesday/blob/main/data/2021/2021-04-20/readme.md))
- **Size:** 7,787 titles, 12 original columns (type, title, director, cast, country, date_added, release_year, rating, duration, listed_in, description)

## Tools & Libraries
- Python
- Pandas — data cleaning & transformation
- Matplotlib & Seaborn — data visualization
- Jupyter Notebook

## Project Workflow
1. **Data Loading & Inspection** — reviewed structure, data types, and missing values
2. **Data Cleaning** — handled missing values in `country`, `director`, `cast`; converted `date_added` to datetime; engineered `year_added` and `month_added` features
3. **Data Transformation** — exploded multi-valued `listed_in` (genre) and `country` fields for granular analysis
4. **Exploratory Analysis**
   - Movies vs TV Shows split
   - Top 10 genres by title count
   - Content additions by year and month
   - Top 10 content-producing countries
   - Content ratings distribution
   - Movie duration distribution
5. **Insights & Takeaways** — summarized key findings from each analysis

## Key Findings
- Movies make up ~69% of the catalog vs. ~31% TV Shows
- **International Movies**, **Dramas**, and **Comedies** are the most common genres
- Content additions peaked in **2019** before declining in 2020-2021
- The **United States** and **India** are the top two content-producing countries
- **TV-MA** and **TV-14** are the most common content ratings
- Average movie duration is approximately **99 minutes**

## Repository Structure
```
Netflix-Data-Analytics/
├── Netflix_EDA.ipynb        # Main analysis notebook
├── netflix_titles.csv       # Dataset
├── charts/                  # Exported visualizations
├── requirements.txt         # Python dependencies
└── README.md
```

## How to Run
```bash
pip install -r requirements.txt
jupyter notebook Netflix_EDA.ipynb
```

## Author
**Shaik Baji Shaida**
[LinkedIn](https://www.linkedin.com/in/bajishaida/) | [GitHub](https://github.com/Baji-Shaida)
