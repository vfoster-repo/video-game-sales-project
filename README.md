# Video Game Sales Analysis

Forecasting 2017 sales trends for strategic advertising campaigns using historical video game sales data.

## Project Overview

**Business Context:** Understanding the gaming industry landscape for investment or publishing decisions.

This project analyzes video game sales data from 2013-2016 to identify patterns that determine a game's success. Working with historical sales data from the online store Ice, I analyzed platform lifecycles, genre performance, and regional market preferences to help plan future advertising campaigns for 2017.

## What This Demonstrates

### Learning Challenge
- Gaming industry dynamics and platform ecosystems
- Time-series analysis across multiple regions
- Handling categorical data (genres, platforms, publishers)

### Problem-Solving Process
1. **Market Research**: Investigated how the gaming industry works (platforms, regions, genres)
2. **Multi-Dimensional Analysis**: Examined sales across time, geography, and product categories
3. **Trend Identification**: Discovered platform lifecycles and regional preferences
4. **Insight Synthesis**: Connected multiple findings into a coherent market narrative

### Professional Outcome
- Delivered insights that could inform publishing strategy, platform prioritization, or market entry decisions
- Demonstrated ability to quickly become conversant in a new industry
- Created visualizations that make 40+ years of data immediately accessible

### Tools Utilized
- VS Code with GitHub Copilot for development
- Jupyter Notebook for interactive analysis
- Git/GitHub for version control

## Key Objectives

- Identify platforms with growth potential for 2017
- Analyze genre performance across different markets
- Understand regional preferences in North America, Europe, and Japan
- Test hypotheses about user ratings across platforms and genres
- Provide data-driven recommendations for advertising strategy

## Dataset

The analysis uses video game sales data spanning 1980-2016:

| Field | Description |
|-------|-------------|
| `name` | Game title |
| `platform` | Gaming platform (PS4, XOne, PC, etc.) |
| `year_of_release` | Release year |
| `genre` | Game genre (Action, Sports, etc.) |
| `na_sales` | Sales in North America (millions) |
| `eu_sales` | Sales in Europe (millions) |
| `jp_sales` | Sales in Japan (millions) |
| `other_sales` | Sales in other regions (millions) |
| `critic_score` | Metacritic score (0-100) |
| `user_score` | User rating (0-10) |
| `rating` | ESRB rating (E, T, M, etc.) |

**Total Records:** 16,715 video games

## Key Findings

### Platform Insights
- **PS4 dominance**: 49% growth and 314M in total sales (2013-2016)
- **Generational transition**: Previous generation platforms (PS3, X360) experienced 87-89% decline
- **Platform lifecycle**: Gaming platforms typically last 10-12 years before rapid decline
- **Regional preferences**: PS4 leads in North America and Europe; 3DS dominates Japan (48% market share)

### Genre Performance
- **Action games**: Dominant with 29.5% market share globally
- **Shooter games**: Highest average sales per title (1.25M)
- **Regional differences**: Role-Playing games lead in Japan (36% market share)

### Review Impact
- **Critic scores**: Moderate positive correlation with sales (0.407)
- **User scores**: Minimal correlation with sales (-0.032)
- **Implication**: Professional reviews influence purchasing more than user ratings

### Regional Market Analysis
- **ESRB ratings**: M-rated games perform best in NA/EU; T-rated games lead in Japan
- **Cultural preferences**: Distinct differences between Western and Japanese markets
- **Platform distribution**: PS4 (36% in Europe), XOne (emphasis in NA), 3DS (48% in Japan)

## Methodology

1. **Data Preparation**
   - Cleaned and standardized 16,715 video game records
   - Handled missing values (critic scores, user scores, ESRB ratings)
   - Converted data types (user_score from text to numeric)
   - Created total_sales column

2. **Temporal Analysis**
   - Analyzed game releases from 1980-2016
   - Identified platform lifecycles (10-12 years)
   - Selected relevant period (2013-2016) for forecasting

3. **Platform & Genre Analysis**
   - Evaluated sales trends and market share
   - Created heatmaps and visualizations
   - Analyzed platform decline and growth patterns

4. **Regional Profiling**
   - Compared preferences across North America, Europe, and Japan
   - Analyzed ESRB rating impact by region
   - Identified genre preferences by market

5. **Statistical Testing**
   - Hypothesis 1: Xbox One vs PC user ratings (t-test)
   - Hypothesis 2: Action vs Sports genre ratings (t-test)
   - Alpha threshold: 0.05

## Recommendations for 2017

1. **Focus on PS4 and XOne** - only growing platforms
2. **Prioritize Action and Shooter genres** globally
3. **Customize by region**: PS4 in Europe, XOne in NA, 3DS in Japan
4. **Feature games with high critic scores** in advertising
5. **Target M-rated content** in Western markets, T-rated in Japan
6. **Avoid previous-generation consoles** (PS3, X360, Wii)

## Technologies Used

- **Python 3.x**
- **pandas** - Data manipulation and analysis
- **NumPy** - Numerical computing
- **matplotlib** - Data visualization
- **seaborn** - Statistical data visualization
- **SciPy** - Statistical hypothesis testing
- **Jupyter Notebook** - Interactive development environment

## Repository Structure

```
video-game-sales-project/
│
├── README.md
├── requirements.txt
├── index.html
├── video-game-sales-analysis.ipynb
└── datasets/
    └── games.csv
```

## How to Run

### Prerequisites
```bash
python 3.7+
```

### Installation

1. Clone the repository:
```bash
git clone https://github.com/vfoster-code/video-game-sales-project.git
cd video-game-sales-project
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Launch Jupyter Notebook:
```bash
jupyter notebook video-game-sales-analysis.ipynb
```

Alternatively, view the pre-rendered HTML file in your browser:
```bash
open index.html
```

## Skills Demonstrated

- Data cleaning and preprocessing
- Exploratory data analysis (EDA)
- Temporal analysis and trend identification
- Statistical hypothesis testing
- Data visualization with matplotlib and seaborn
- Business insights interpretation
- Regional market analysis
- Python programming for data science

## License

This project was completed as part of the TripleTen AI/ML Engineering program.

## Author

**Victor Foster**
- GitHub: [@vfoster-repo](https://github.com/vfoster-repo)
- LinkedIn: [Victor Foster](https://linkedin.com/in/vfoster-connect)
- Email: victorfoster@hotmail.com

## Acknowledgments

- TripleTen  AI/ML Engineering Program Sprint 6 "Project: Video Game Sales Forecasting"

---

If you found this project helpful, please consider giving it a star!
