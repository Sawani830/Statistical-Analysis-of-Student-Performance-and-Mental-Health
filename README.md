
# Statistical Analysis of Student Performance and Mental Health

This repository contains the Jupyter Notebook **Stats Project Final (1).ipynb**, which documents an extensive statistical analysis using the `student-mat.csv` dataset. The project investigates the relationships between students’ family backgrounds (e.g., living with both parents, single parents, or being an orphan), various lifestyle factors, and their reported mental health and academic outcomes.

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset Description](#dataset-description)
- [Methodology](#methodology)
  - [Data Cleaning and Preparation](#data-cleaning-and-preparation)
  - [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
  - [Statistical Testing](#statistical-testing)
  - [Results Interpretation](#results-interpretation)
- [How to Run the Analysis](#how-to-run-the-analysis)
- [Technologies Used](#technologies-used)
- [Future Work](#future-work)
- [Acknowledgments](#acknowledgments)
- [License](#license)

## Project Overview

This project aims to explore how different family environments impact student mental health and academic performance. Using the `student-mat.csv` dataset, the analysis includes data cleaning, descriptive and inferential statistics, and hypothesis testing. The study focuses on how family composition—whether a student lives with both parents, a single parent, or neither—affects self-reported health indicators and academic grades (G1, G2, and G3). Additionally, the project examines lifestyle variables such as free time, social outings, and alcohol consumption (both during weekdays and weekends) to understand their potential influence on mental well-being.

## Dataset Description

The analysis is based on the **student-mat.csv** file, which contains data on students’ academic performance, demographic information, family background, and lifestyle variables. Key variables include:

- **Demographics & Background:**
  - `school`: School identifier (e.g., GP)
  - `sex`: Gender of the student
  - `age`: Age of the student
  - `address`: Type of home address (urban or rural)
  - `famsize`: Family size (e.g., GT3, LE3)
  - `Pstatus`: Parent cohabitation status (living together “T” or apart “A”)
  - `Medu` & `Fedu`: Mother’s and father’s education levels
  - `Mjob` & `Fjob`: Mother’s and father’s job type
  
- **Academic Performance:**
  - `G1`, `G2`, `G3`: Grades for three periods

- **Lifestyle and Personal Factors:**
  - `famrel`: Quality of family relationships
  - `freetime`: Amount of free time after school
  - `goout`: Frequency of going out with friends
  - `Dalc` & `Walc`: Alcohol consumption on weekdays and weekends
  - `health`: Self-reported health status
  - `absences`: Number of school absences

The dataset provides a unique opportunity to analyze how family structure and lifestyle aspects might correlate with students’ mental health (proxied by the `health` variable) and their academic results.

## Methodology

### Data Cleaning and Preparation

- **Preprocessing:**  
  The notebook details the cleaning process which includes handling missing values, correcting inconsistencies, and transforming categorical variables into appropriate formats for analysis.
- **Outlier Detection:**  
  Identification and treatment of outliers to ensure robustness of subsequent statistical tests.
- **Feature Engineering:**  
  Derivation of additional metrics where necessary and preparing variables for group comparisons (e.g., categorizing family types).

### Exploratory Data Analysis (EDA)

- **Descriptive Statistics:**  
  Summary statistics (mean, median, standard deviation) are computed for academic scores, self-reported health, and lifestyle variables.
- **Visualization:**  
  Histograms, box plots, and scatter plots are used to visualize the distribution of key variables and to explore correlations between:
  - Family background variables and academic outcomes.
  - Lifestyle factors (such as alcohol consumption and free time) and self-reported health.

### Statistical Testing

The project experiments with several statistical tests to verify the impact of family environment on mental health and academic performance:

- **Group Comparisons:**  
  T-tests and ANOVA are applied to compare means between students from different family backgrounds.
- **Correlation Analysis:**  
  Pearson or Spearman correlation tests are used to quantify the relationships between lifestyle factors, academic scores, and the self-reported health measure.
- **Hypothesis Testing:**  
  Null and alternative hypotheses are defined to test for significant differences or associations, with results interpreted at appropriate significance levels.

### Results Interpretation

- **Key Findings:**  
  The notebook summarizes findings regarding how family composition correlates with mental health indicators and academic performance.  
- **Statistical Significance:**  
  Details on p-values and confidence intervals are provided to assess the reliability of the observed effects.
- **Discussion:**  
  Interpretation of how factors like parental status, family relationship quality, and lifestyle choices influence student outcomes, and discussion on potential implications for educators and policymakers.

## How to Run the Analysis

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/<your_username>/<repository_name>.git
   cd <repository_name>
   ```

2. **Set Up a Python Environment (optional but recommended):**

   ```bash
   python3 -m venv env
   source env/bin/activate    # For Windows: env\Scripts\activate
   ```

3. **Install Required Packages:**

   If a `requirements.txt` is included, run:

   ```bash
   pip install -r requirements.txt
   ```

   Alternatively, install the necessary libraries manually (e.g., `pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy`).

4. **Launch Jupyter Notebook:**

   ```bash
   jupyter notebook
   ```

5. **Open and Run the Notebook:**

   Open **Stats Project Final (1).ipynb** and run each cell sequentially to reproduce the analysis.

## Technologies Used

- **Python** – Primary programming language for statistical analysis.
- **Jupyter Notebook** – Interactive environment for documenting and executing the analysis.
- **Pandas & NumPy** – Data manipulation and numerical computation.
- **Matplotlib & Seaborn** – Data visualization.
- **SciPy** – Statistical tests and hypothesis testing.

## Future Work

- **Additional Variables:**  
  Explore adding further demographic or social variables to enrich the analysis.
- **Advanced Modeling:**  
  Consider using multivariate regression or machine learning techniques for predictive analysis.
- **Longitudinal Analysis:**  
  If additional data over time becomes available, perform a longitudinal study on student outcomes.

## Acknowledgments

- Appreciation is extended to instructors, peers, and dataset providers who supported this analysis.
- Acknowledgment of any external resources, tutorials, or libraries that informed the methodology.
