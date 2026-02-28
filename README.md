# Parental Education and Student Academic Success

**Course:** 602 - Data 602 Statistical Data Analysis  

This project investigates the influence of parental education on student academic performance and graduation outcomes using the **Student Performance (PIP)** dataset from the Polytechnic Institute of Portalegre. The study aims to determine whether students whose parents have higher educational qualifications perform better academically and are less likely to drop out than those whose parents have lower qualifications. Understanding this relationship can help inform targeted support strategies for students from first-generation or lower-education backgrounds.

## Tech Stack and Libraries Used

- **R / RStudio / R Markdown** – Data analysis, visualization, and reporting  
- **tidyverse (dplyr, ggplot2)** – Data wrangling and plotting  
- **mosaic** – Descriptive statistics (favstats)  
- **stats** – t-tests, chi-square tests, permutation tests  
- **Bootstrap and permutation methods** – Resampling techniques for robust inference  

**Dataset:** [Student Performance (PIP) - Kaggle](https://www.kaggle.com/datasets/mikhail1681/student-performance-pip)

## Methodology

1. **Data Preparation**
   - Created a new column `overall_marks` by summing first and second semester grades.  
   - Selected relevant variables: `semester1`, `semester2`, `overall_marks`, and `Parents_Qualification`.  
   - Stratified data into two groups based on parental education:
     - **Group 0:** Parents with at most high school education  
     - **Group 1:** Parents with post-secondary or higher education  

2. **Descriptive Statistics**
   - Summarized the distribution of overall marks and semester grades.  
   - Visualized with bar plots, boxplots, and normal probability plots.

3. **Statistical Tests**
   - **Welch’s t-test (one-tailed):** Compare mean overall grades between groups.  
   - **Bootstrap estimation:** Resampling to estimate mean grade differences with confidence intervals.  
   - **Permutation test:** Non-parametric test comparing group means.  
   - **Chi-square test of independence:** Examined association between parental education and student dropout.

## Results and Insights

- **Descriptive Analysis:** Both parental education groups had similar grades distributions; differences are minimal.  
- **Statistical Testing:**  
  - t-test: p-value = 0.6789 → no significant difference in overall marks  
  - Bootstrap: mean difference ≈ -0.089; 95% CI includes 0 → negligible difference  
  - Permutation test: p-value = 0.692 → no significant effect  
  - Chi-square test: p-value = 0.522 → dropout status independent of parental education  

**Conclusion:**  
Parental education does not significantly impact student academic performance or dropout likelihood in this dataset. Any observed differences are minor and likely due to random variation. Future research could include additional factors such as socioeconomic status, study habits, school type, and family support to better understand academic success determinants.

## Group Members

- Ishwarya Rani Murali  
- Sanjay Sundar 
- Simrat Toor  
- Shreyaa Sathesh Kumar 
