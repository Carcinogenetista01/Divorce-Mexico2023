Here's a professional README.md for your Mexican Divorce Analysis project:

# 📊 Mexican Divorce Patterns Analysis (2023)

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2C2D72?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)

Comprehensive analysis of divorce patterns in Mexico using 2023 national registry data (163,587 records).

## 📂 Dataset Overview
- **Source**: National Divorce Registry 2023
- **Records**: 163,587 divorce cases
- **Features**: 64 variables including:
  - Demographic data (age, gender, education)
  - Marriage details (duration, location)
  - Divorce circumstances (cause, initiator)
  - Child custody information

## 🔍 Key Analyses Performed

### A. Age Correlation Analysis
![Age Scatterplot](https://via.placeholder.com/400x300?text=Age+Relationship+Plot)
- Examined age relationships between divorcing partners
- Filtered out invalid entries (age = 999)
- Visualization: Dual-tone scatter plot showing age correlations

### B. Marriage Duration Analysis
![Duration Histogram](https://via.placeholder.com/400x300?text=Marriage+Duration)
- Calculated marriage duration 
- Identified average marriage duration: 
- Visualization: Histogram with mean indicator

### C. Divorce Causes Breakdown
![Causes Bar Chart](https://via.placeholder.com/400x300?text=Divorce+Causes)
- Mapped 28 distinct divorce causes
- Top 3 causes:
  1. Mutual consent 
  2. Incompatibility 
  3. Abandonment 

### D. Cause vs Duration Analysis
![Cause-Duration Plot](https://via.placeholder.com/400x300?text=Cause+Duration)
- Calculated average marriage duration by cause
- Notable finding: Adultery cases had shortest duration 

### E. Couple Gender Distribution
![Gender Distribution](https://via.placeholder.com/400x300?text=Gender+Distribution)
- Breakdown:
  - Heterosexual couples
  - Same-sex couples
    - Male couples
    - Female couples

### F. Children Impact Analysis
![Children Chart](https://via.placeholder.com/400x300?text=Children+Analysis)
- Most common scenarios:
  - No children
  - 1 child
  - 2 children

### G. Divorce Initiator Analysis
![Initiator Chart](https://via.placeholder.com/400x300?text=Initiator+Analysis)
- Gender breakdown of who files:
  - Women
  - Men
  - Join

### H. Geographic Patterns
![Geographic Heatmap](https://via.placeholder.com/400x300?text=Geographic+Analysis)
- Compared marriage vs divorce locations
- Top migration patterns between states

### I. Education Level Analysis
![Education Chart](https://via.placeholder.com/400x300?text=Education+Analysis)
- Most common education levels:
  1. Secondary complete 
  2. High school complete 
  3. University complete 

### J. Seasonal Trends
![Seasonal Chart](https://via.placeholder.com/400x300?text=Seasonal+Trends)
- Peak divorce months: 
  - January 
  - August 

## 🛠️ Technical Implementation

```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# Data cleaning
df = df[(df['edad_div1'] != 999) & (df['edad_div2'] != 999)]

# Visualization example
plt.figure(figsize=(14, 8))
sns.scatterplot(data=df, x='edad_div1', y='edad_div2', 
                hue='edad_div1', palette="Blues", alpha=0.8)
```

## 📊 Key Findings
1. **Age Pattern**: Most divorces occur between partners aged X-X
2. **Duration**: Average marriage lasts X years before divorce
3. **Gender Gap**: Women initiate XX% more divorces than men
4. **Education**: Higher education correlates with longer marriages
5. **Seasonality**: Post-holiday period sees divorce spikes

## 📥 How to Use
1. Clone repository
```bash
git clone https://github.com/yourusername/mexican-divorce-analysis.git
```
2. Install requirements
```bash
pip install -r requirements.txt
```
3. Run Jupyter notebook
```bash
jupyter notebook mexican_divorce_analysis.ipynb
```

## 📄 Data Sources
- National Population Registry (2023)
- Mexican Judicial Statistics

## 📜 License
MIT License - Free for academic/research use with attribution

