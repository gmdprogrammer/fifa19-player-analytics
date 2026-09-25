**FIFA 19 — What Makes a Top Football Player?** ⚽📊

A statistical analysis of 18,147 real professional footballers from FIFA 19, exploring what actually predicts player quality — and answering the questions scouts, managers, and agents care about most.

**The story:** EA Sports collected detailed data on 18,000+ real professional footballers for FIFA 19. This project digs into that data to answer: *Does foot preference affect rating? Do forwards outperform defenders? What best predicts a player's market value?*


## 🎯 Project Goal

Explore, test, visualize, and brief a scouting team using real hypothesis testing and correlation analysis — not just intuition.

## 📂 Dataset

- **Source:** EA Sports / Kaggle FIFA 19 Complete Player Dataset
- **Size:** 18,147 players × 20 columns (after cleaning)
- **Key columns:** `Age`, `Overall`, `Potential`, `Preferred Foot`, `Skill Moves`, `Dribbling`, `ShortPassing`, `BallControl`, `Finishing`, `Stamina`, `Strength`, `Value_EUR`, `Wage_EUR`, `pos_group` (simplified to GK / Defender / Midfielder / Forward)

## 🛠️ Methodology

| Step | What was done |
|---|---|
| **1. Exploratory Data Analysis** | Shape, missing values, summary statistics, group breakdowns by position and preferred foot |
| **2. Visualization** | Histograms, boxplots, scatter plot with trend line, grouped bar charts |
| **3. Normality Checks** | Shapiro-Wilk tests and Q-Q plots to decide between parametric and non-parametric tests |
| **4. Group Comparisons** | Mann-Whitney U, Kruskal-Wallis, and Tukey post-hoc tests |
| **5. Correlation Analysis** | Pearson/Spearman correlation heatmap and a p-value significance matrix |
| **6. Categorical Relationships** | Chi-Square tests on Preferred Foot and Skill Tier vs. Position |
| **7. Summary & Brief** | Consolidated results table, p-value chart, and a scouting brief with concrete recommendations |

## 🔑 Key Findings

- **Skill beats strength.** Ball control and passing are stronger predictors of `Overall` rating than physical attributes like `Strength`.
- **Forwards ≈ Defenders.** Their average `Overall` ratings are statistically indistinguishable (p = 0.96).
- **Goalkeepers rate ~2 points lower** on average than outfield players — largely a scoring-scale effect, not a talent gap.
- **Potential declines with age**, supporting the case for investing in younger players.
- **Left-footed players rate marginally higher** than right-footed players (+0.7 pts) — statistically real, but a small effect given the sample size.
- **7 of 8 hypothesis tests** rejected the null hypothesis; effect sizes were checked alongside p-values given the large sample.

## 📁 Repository Contents

```
├── Solution_of_fifa_challenge.ipynb   # Full analysis notebook
├── README.md                          # This file
```

## 🚀 How to Run

1. Clone the repository
   ```bash
   git clone https://github.com/<your-username>/<repo-name>.git
   cd <repo-name>
   ```
2. Install dependencies
   ```bash
   pip install numpy pandas matplotlib seaborn scipy statsmodels
   ```
3. Open and run the notebook
   ```bash
   jupyter notebook Solution_of_fifa_challenge.ipynb
   ```
   Or open it directly in [Google Colab](https://colab.research.google.com/).

## 🧰 Tools & Libraries

`Python` · `pandas` · `NumPy` · `Matplotlib` · `Seaborn` · `SciPy` · `statsmodels`

## 👤 Author

**Ghulam Mohayud Din**
- LinkedIn: [linkedin.com/in/thegmd](https://linkedin.com/in/thegmd)
- GitHub: [github.com/gmdprogrammer](https://github.com/gmdprogrammer)
- Email: gmd.programmer@gmail.com

---

*The beautiful game, made more beautiful with data.* ⚽📈
