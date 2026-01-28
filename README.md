**Parental Education and Student Academic Success**

**Overview:**

This project analyzes the impact of parental education level on student academic performance and graduation/dropout status using statistical inference methods. The goal is to assess whether students with more highly educated parents perform better academically and are less likely to drop out.

**Dataset:**
Source: Student Performance (PIP) Dataset
Origin: UCI Machine Learning Repository (via Kaggle)
Population: Students from the Polytechnic Institute of Portalegre
License: CC BY 4.0
Time Frame: 2005–2006 academic year

**Variables:**
Parental Education: Binary (1 = post-secondary or higher, 0 = high school or lower)
Academic Performance: Overall marks (continuous)
Outcome: Graduation / dropout status (categorical)

**Methods:**
One-tailed two-sample t-test
Bootstrap estimation of mean grade differences
Two-tailed permutation test (4,999 permutations)
Chi-square test for parental education vs. dropout status
Significance level: α = 0.05

**Purpose:**
To quantify how parental education relates to student success and provide insights for supporting first-generation and at-risk students.
