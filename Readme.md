# How User Behavior Drives Movie Ratings

## Overview
This project presents an **exploratory data analysis (EDA)** of the **MovieLens 20M dataset**, focusing on how user behavior has evolved over two decades and how different types of users interpret and express opinions through ratings and tags.

Rather than treating ratings as objective measures of content quality, this analysis examines them as **behavioral signals**, shaped by user engagement, sentiment bias, and platform maturity.

The goal is to move beyond descriptive trends and provide **actionable insights** that stakeholders can use to interpret ratings, engagement metrics, and audience feedback more effectively.

---

## Key Questions Explored
- How has user activity (ratings and tags) evolved over time?
- Why do aggregate ratings change even when content does not?
- Are all users equally represented in platform-level metrics?
- Can users be grouped into behavioral **“taste tribes”**?
- How do these tribes differ in how they rate genres?

---

## Dataset
- **Source:** MovieLens 20M Dataset (GroupLens Research)
- **Time Span:** 1995–2015

### Files Used
- `movies.csv`
- `ratings.csv`
- `tags.csv`
- `links.csv`
- `genome-tags.csv`
- `genome-scores.csv`

---

## Key Insights
- Aggregate ratings are dominated by highly active users, not necessarily the most satisfied ones.
- Less active users consistently rate more positively but are underrepresented in summary metrics.
- Declines in rating and tagging activity align with platform maturation and industry-wide shifts toward implicit feedback.
- Genre performance varies significantly depending on *who* is rating, not just *what* is being rated.

---

## Project Structure
```text
movielens/
├── data/
│   ├── raw_data/
│   │   ├── genome-scores.csv
│   │   ├── genome-tags.csv
│   │   ├── links.csv
│   │   ├── links_clean.csv
│   │   ├── movies.csv
│   │   └── ratings.csv
│   └── cleaned_data/
│       ├── genome_scores_clean.csv
│       ├── genome_tags_clean.csv
│       ├── movies_clean.csv
│       ├── movies_genres_clean.csv
│       ├── ratings_clean.csv
│       └── tags_clean.csv
├── data_cleaning/
│   ├── genome_scores.ipynb
│   ├── genome_tags.ipynb
│   ├── links.ipynb
│   ├── movies.ipynb
│   └── ratings.ipynb
├── EDA/
│   ├── obs1.ipynb   # Platform-level trends: users, ratings, tags over time
│   ├── obs2.ipynb   # Dynamics of tags vs ratings
│   ├── obs3.ipynb   # Genre-level rating distribution analysis
│   └── obs4.ipynb   # User clustering & Taste Tribes analysis
├── report/
│   └── movielens_eda.pdf
├── .gitignore
└── README.md
