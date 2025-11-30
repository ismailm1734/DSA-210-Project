# DSA-210-Project
# Predicting Tennis Match Winners with Historical ATP Statistics

## Motivation
The goal of this project is to explore whether historical player and match statistics can be used to predict tennis match outcomes. Tennis is a data-rich sport, making it an ideal domain for applying data analysis and machine learning approaches. By identifying key performance indicators (such as serve rating, aces, and unforced errors), this project aims to understand the factors that influence a player's likelihood of winning a match.

## Research Questions
- Which performance statistics (aces, serve percentage, unforced errors, etc.) are most predictive of match outcomes?  
- Does the playing surface (hard, clay, or grass) influence a player's probability of winning?  
- Can a simple classification model accurately predict the winner of a professional tennis match?

## Data Source
The project will use a public ATP tennis match dataset from Kaggle:  
🔗 [ATP Matches Dataset (1968–2023)](https://www.kaggle.com/datasets/gmadevs/atp-matches-dataset-19682023)

The project will use a public ATP tennis match dataset from Kaggle, which includes detailed match-level statistics such as:
- Aces and double faults  
- First-serve percentage and points won  
- Break points  
- Winners and unforced errors  
- Surface type (hard, clay, grass)  
- Match duration and player ranking  

The dataset contains thousands of matches across many years, allowing for robust predictive analysis and feature exploration.

## Planned Methodology
The workflow will include data cleaning, feature inspection, and descriptive statistical analysis to identify performance patterns and key match drivers. Following exploratory analysis, the dataset will be formatted for a binary classification task, where the target variable represents match outcome (win/loss). Initial baseline models such as logistic regression will be implemented, followed by evaluation using accuracy and performance metrics. Future extensions may include ensemble models such as random forests if time permits.

## Expected Outcomes
- Discovery of the most influential performance indicators in determining match outcomes  
- A baseline machine learning model capable of predicting match winners with reasonable accuracy  
- Visual representations showing relationships between features such as serve performance, surface type, and match results
  
## Limitations and Future Work
This project relies on publicly available historical ATP match data, which may include missing or imbalanced records for certain player levels, surfaces, or match periods. Additionally, the analysis does not currently include player-specific contextual variables such as injury history, fatigue levels, psychological factors, or weather and crowd conditions. As the dataset is observational, causality cannot be inferred — results represent correlations rather than deterministic effects.

**Future Work**  
To enhance model accuracy and depth, future work could incorporate real-time player statistics, physical metrics (such as serve speed distributions and movement tracking), and external contextual data such as weather conditions or tournament stage. Advanced models, including gradient boosting or neural networks, could also be explored. Finally, collecting and analyzing personal tennis performance data could offer a more individualized extension of this study.

**Phase 2: Exploratory Data Analysis (EDA) Summary
During Phase 2, I examined the ATP match dataset and explored several basic patterns in the data. I looked at the general structure of the dataset, missing values, and the distribution of key performance variables such as aces, double faults, and surface types. I also created visualizations to understand how features behave, including histograms, a correlation heatmap, and a surface distribution chart. The dataset shows clear differences between winners and losers in multiple areas, especially in serve-related statistics.
Hypothesis Testing Summary
I performed several hypothesis tests to check whether some match statistics differ between winners and losers.
H1: Winners and losers differ in first-serve points won.
H2: Winners and losers differ in break points won.
H3: The playing surface is related to the probability that the higher-ranked player wins.
The tests show that some performance metrics have statistically meaningful differences between winners and losers, while surface also plays a role in match outcomes. These findings are consistent with the general understanding of tennis, where serve performance and break-point conversion are important factors.
