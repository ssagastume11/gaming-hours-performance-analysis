![GitHub Repo Size](https://img.shields.io/github/repo-size/ssagastume11/gaming-hours-performance-analysis)
![Last Commit](https://img.shields.io/github/last-commit/ssagastume11/gaming-hours-performance-analysis)

# 🎮 Gaming Hours vs Academic & Work Performance Analysis

This project analyzes how gaming habits relate to academic and workplace performance outcomes. Using behavioral, lifestyle, and performance metrics, the analysis explores whether gaming has a positive, negative, or neutral impact on productivity, focus, stress, sleep, and overall performance across different occupations and gaming patterns.

---

## 📦 Dataset

**Source**: [Gaming Hours vs Academic & Work Performance Dataset]([https://www.kaggle.com/datasets/ahmeduzaki/global-earthquake-tsunami-risk-assessment](https://www.kaggle.com/datasets/prince7489/gaming-hours-vs-academic-and-work-performance)  
**Platform**: Kaggle (public behavioral dataset)

**Location**: Stored in the `data/` folder  
**Filename**: `gaming_performance_cleaned.csv`

**Key Fields Include**:
- User ID
- Age, Gender, Occupation
- Game Type
- Daily & Weekly Gaming Hours
- Primary Gaming Time
- Sleep Hours
- Stress Level
- Focus Level
- Academic or Work Score
- Productivity Level

---

## 🔍 Business Task

The objective of this analysis is to determine whether gaming habits influence academic and workplace performance by:

- Evaluating relationships between gaming duration and performance scores
- Comparing moderate vs heavy gaming behaviors
- Examining the role of sleep, stress, and focus
- Identifying patterns across occupations and gaming schedules

---

## 📊 Tools & Technology

- **Google BigQuery** – Data cleaning, transformation, and aggregation
- **SQL** – Structured analysis queries
- **Tableau Public** – Interactive dashboard visualization
- **Google Slides** – Stakeholder-ready presentation
- **Git & GitHub** – Version control and project sharing

---

## 📁 Project Structure

```plaintext
gaming-hours-performance-analysis/
├── data/
├── sql/
├── visuals/
├── tableau/
├── presentation/
└── README.md
```

---

## 🧮 Sample SQL Query (Gaming Hours vs Performance)

```SQL
SELECT
  performance_category,
  AVG(daily_gaming_hours) AS avg_daily_gaming_hours,
  AVG(sleep_hours) AS avg_sleep_hours,
  AVG(stress_level) AS avg_stress_level,
  AVG(focus_level) AS avg_focus_level,
  AVG(academic_or_work_score) AS avg_performance_score,
  COUNT(*) AS total_users
FROM
  `plenary-ability-463920-b3.gaming_analysis.gaming_performance_cleaned`
GROUP BY
  performance_category
ORDER BY
  avg_performance_score DESC;
```

---

## 📈 Analysis Output

Key visual outputs stored in the visuals/ folder include:

- 🎯 Average gaming hours by performance category
- 😴 Sleep, stress, and focus trends by gaming time
- ⚙️ Productivity differences across primary gaming schedules
- 🧑‍💼 Occupational comparisons of gaming impact

---

## 📊 Interactive Tableau Dashboard

Explore the interactive dashboard analyzing how gaming habits impact academic and workplace performance:

🔗 **Tableau Public Dashboard:**  
[Gaming Hours vs Academic & Work Performance Dashboard](https://public.tableau.com/views/GamingAnalysis_17695234070720/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

This dashboard allows users to interactively explore:
- Gaming duration (daily and weekly)
- Sleep, stress, and focus levels
- Productivity and academic/work performance
- Performance impact categories (Positive, Neutral, Negative)
- Differences across occupations and gaming times

---

## 🧾 Presentation

The final presentation (located in the presentation/ folder) covers:

- Project objective and business questions
- Data preparation and processing steps
- Key analytical insights with visuals
- Actionable recommendations

---

## ✅ Next Steps
- Moderate gaming is generally associated with neutral or slightly positive performance outcomes
- Higher gaming hours often align with increased stress and reduced focus
- Sleep duration strongly influences both academic and workplace performance
- Late-night gaming shows lower average productivity trends

---

## 📌 Recommendations

- Encourage balanced gaming habits rather than elimination
- Promote healthy sleep routines, especially for late-night gamers
- Use performance and wellness metrics to guide productivity strategies
- Monitor gaming behavior patterns alongside stress and focus indicators

---

## 🙌 Acknowledgments
- Dataset courtesy of [Prince Rajak on Kaggle]([https://www.kaggle.com/datasets/ahmeduzaki/global-earthquake-tsunami-risk-assessment](https://www.kaggle.com/datasets/prince7489/gaming-hours-vs-academic-and-work-performance))
- Tools powered by Google Cloud, BigQuery, SQL, Tableau and Google Slides.

---

👨‍💻 Author

**Sergio E. Sagastume**
Data Analyst | SQL | Tableau | R
