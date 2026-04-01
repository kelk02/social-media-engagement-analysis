# Instagram Influencer Engagement Analysis

An exploratory data analysis (EDA) of the top 1000 Instagram influencers, investigating what drives engagement across different countries and content categories.

# Problem Statement
What factors drive engagement (likes, shares, comments) on Instagram? Specifically:
- Which countries produce the most influential creators?
- Which content categories generate the highest average engagement?
- Does audience location affect engagement levels?


# Project Structure
social-media-engagement-analysis/
- data/
│   └── instagram.csv
-notebooks/
│   └── 01_eda.ipynb
- README.md
- .gitignore

# Dataset

Source: Top 1000 Social Media Influencers – Kaggle
Platform: Instagram
Size: ~1000 rows, 7 columns after cleaning
Key variables: Followers, Engagement Average, Authentic Engagement, Country, Category


# Tools Used
Python
Pandas
Matplotlib
Seaborn
Jupyter Notebook


# Data Cleaning Steps
Dropped category_2 column due to 713 missing values (71% of data)
Removed rows with missing country values
Filled missing category_1 values with 'Unknown'
Converted followers, engagement_avg and authentic_engagement from string format (e.g. 1.4M, 637K) to numeric values
Standardised column names to lowercase with underscores


# Key Findings
Finding 1 — Top Countries by Number of Influencers
The United States dominates with nearly 280 influencers, almost double Brazil and India. However the strong presence of Brazil, India and Indonesia highlights that influencer culture is truly global.
Finding 2 — Top Content Categories
Music and Lifestyle are the most common influencer categories, suggesting these are the most popular niches for building a large following on Instagram.
Finding 3 — Engagement by Category
Management & Marketing and Fashion drive the highest average engagement at nearly 2 million per post — almost double lower ranking categories like Photography and Modeling. Aspirational and career-driven content resonates most strongly with audiences.
Finding 4 — Engagement by Country
South Korea leads all countries with an average engagement of nearly 2 million, significantly ahead of France and Indonesia. Notably South Korea outperforms much larger markets like the US, likely driven by the global reach of K-pop and Korean culture.


# How to Run
Clone this repository
bashgit clone https://github.com/kellyk02/social-media-engagement-analysis.git

Install dependencies
bashpip install pandas matplotlib seaborn jupyter

Launch Jupyter Notebook
bashjupyter notebook

Open notebooks/01_eda.ipynb and run all cells
