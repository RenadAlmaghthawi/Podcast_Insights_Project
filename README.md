# 🎧 Podcast Insights: From Data to Recommendation

This project explores user listening behavior on podcast episodes and provides actionable insights based on demographic and categorical analysis. It was developed as part of a data science and AI training task for **Thmanyah**.

## 📁 Dataset Description

The project uses three primary datasets:

- `users.csv`: Contains user demographics (user_id, age, gender, country).
- `episodes.csv`: Contains episode metadata (episode_id, title, category).
- `listens.json`: Logs of user listens (user_id, episode_id, duration_seconds).

## ⚙️ Project Workflow

1. **Data Loading**: Read CSV and JSON files using `pandas`.
2. **Exploratory Data Analysis (EDA)**:
   - Reviewed head, info, and null values for each dataset.
   - Confirmed that all datasets are clean and complete.
3. **Data Merging**:
   - Merged `listens.json` with `users.csv` and `episodes.csv` on shared keys.
4. **Analysis & Visualization**:
   - Identified top podcast categories by number of listens.
   - Compared average listening durations between male and female users using plots.
   - Used `matplotlib` and `seaborn` for visualizations.
5. **Basic Recommendation Method**:
   - Developed a simple recommendation function in Python that suggests 3 podcast episodes for each user based on their most listened-to category.

## 📊 Key Findings

- **Popular Content Trends**: The most listened-to podcast categories are *Society*, *Sports*, and *News*, indicating users' preference for socially engaging and up-to-date content.
- **User Engagement by Gender**: Female listeners demonstrated longer average listening durations than male users, suggesting deeper engagement or stronger content affinity.
- **Less Popular Categories**: Topics like *Religion*, *Politics*, and *Technology* received the least attention, offering potential areas for targeted growth or niche podcast production.
- **Country Trends**:Jordan shows highest engagement, especially in *Society* and *Sports*. Morocco prefers *News*, while UAE has the lowest activity.


## 🚀 How to Run

1. Make sure you have Python 3.x installed.
2. Install required libraries:
   ```bash
   pip install pandas matplotlib seaborn
   ```
3. Place the data files (users.csv, episodes.csv, listens.json) in the same directory
4. Open the Podcast_Insights.ipynb notebook and run all cells

## 💡 Future Work
* Build a personalized podcast recommendation system.
* Add sentiment analysis for episode reviews.

 
