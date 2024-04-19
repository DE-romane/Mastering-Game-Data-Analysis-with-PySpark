# Mastering-Game-Data-Analysis-with-PySpark

#### Data Source
📂 **Video Game Sales Dataset:** [Kaggle - Video Game Sales](https://www.kaggle.com/gregorut/videogamesales)

📂 **Steam Video Games Traffic Dataset:** [Kaggle - Steam Video Games](https://www.kaggle.com/tamber/steam-video-games)

#### Objective
🔍 The aim of this analysis was to wrangle, refine, and explore two datasets: "Video Game Sales" and "Video Games Traffic on Steam". The goal was to uncover correlations between global sales figures of video games and their viewership on Steam.

#### 1. Data Overview 📊

**Video Game Sales Dataset:**
- 📈 **Rows:** 16,598
- 📊 **Columns:** 11
- 💡 **Data Types:** Integer, String, Double
- 🛠 **Issues Identified:** Year column is stored as string instead of integer.

**Video Games Traffic Dataset:**
- 📈 **Rows:** 199,999
- 📊 **Columns:** 5
- 💡 **Data Types:** Integer, String, Double
- 🛠 **Issues Identified:** First row contains header values, irrelevant "0" column.

#### 2. Data Cleaning and Preprocessing 🛠

**Video Game Sales Dataset:**
- 🔄 Converted the "Year" column from string to integer.
- 🧹 Removed duplicate rows. (Duplicates: 16,598)
- ✅ No null or missing values found.

**Video Games Traffic Dataset:**
- 🧹 Removed the first row as it contained header values.
- 🧹 Removed duplicate rows. (Duplicates: 199,292)
- 🗑 Removed the irrelevant "0" column.
- ✅ No null or missing values found.

#### 3. Correlation Analysis 📈

- 📊 Calculated correlation between global sales and viewership.
- 📉 **Result:** Weak Positive Correlation (0.0247)
- 📈 As viewership increases, there's a slight tendency for global sales to increase.
- 🤔 However, the correlation is relatively low, indicating other influencing factors on video game sales.

#### 4. Dataset Merge 🔄

- 🔄 Merged datasets based on common columns "Name" and "game-title".
- 📊 **Result:** Merged Dataset
  - 📈 **Rows:** 85,114
  - 📊 **Columns:** 15

#### 5. Exploratory Data Analysis 📊

**Genre-wise Sales:**
- 🕹 Action games dominate global sales, followed by shooter games.

**Global Sales Distribution:**
- 🌍 Most games have sales between 0 and 2 million units, with some outliers.

**Global Sales vs. Value:**
- 💰 Positive relationship between global sales and value.

**Platform Impact:**
- 🎮 Different platforms exhibit varied sales performances.

**Outliers:**
- 🚀 Certain platforms achieve exceptionally high global sales.

**Sales Trends Over Years:**
- 📈 General increasing trend in video game sales across regions.

**Top 5 Publishers:**
- 🥇 Take-Two Interactive, Electronic Arts, Ubisoft, Bethesda Softworks, and Vivendi Games.

**Most Played Games, Genres, and Publishers:**
- 🎮 Terraria, Counter-Strike, Grand Theft Auto V lead in playtime.
- 🕹 Action, Shooter, Role Playing are top played genres.
- 🏢 Take-Two Interactive, 505 Games, Electronic Arts lead in published games.

**Correlations:**
- 📊 Higher-ranked games tend to have higher sales.
- 📉 Weak negative correlation between Year and Rank.

**Global Sales and Viewership:**
- 🌐 Weak positive correlation between global sales and viewership.

#### Conclusion 

Based on the analysis, a weak positive correlation between global game sales and Steam viewership was found. However, this suggests that viewership alone doesn't significantly impact sales. Marketing, quality, pricing, and platform availability likely play more significant roles. 🚀
