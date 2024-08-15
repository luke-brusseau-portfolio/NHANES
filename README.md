# NHANES
NHANES Data Analysis/Data Mining


Goal: Use Data Analytics and Data Mining to try and find key factors that lead to depression

Group Members: Matthew Guo, Ethan Oly

Intro

This project delves into the connection between various health indicators and depression, using advanced statistical methods to uncover patterns within the NHANES dataset. By applying logistic regression, Principal Component Analysis (PCA), K-means clustering, and tree-based methods, we turned complex health data into meaningful insights. Each method helps to better understand the different factors contributing to depression, showing how quantitative data can be used to predict mental health outcomes. This analysis not only reveals important relationships but also highlights the challenges and opportunities in using these techniques to support public health efforts.

Skills

Statistical Modeling: Applying logistic regression to analyze relationships between health indicators and depression.

Dimensionality Reduction: Utilizing Principal Component Analysis (PCA) to simplify complex datasets.

Clustering: Implementing K-means clustering to identify subgroups within the data.

Data Classification: Developing tree-based models to classify and predict depression outcomes.

Data Imbalance Handling: Addressing class imbalance through techniques like upsampling to improve model accuracy.

Tools

R Programming Language: For performing statistical analyses, including logistic regression, PCA, K-means clustering, and tree-based methods.

ggplot2: For data visualization to create plots and charts that illustrate key findings.

Caret Package: For handling data preprocessing, model training, and cross-validation, particularly in addressing class imbalances.

R Markdown: For compiling the analysis into a reproducible report format, combining code, results, and commentary.

Step-by-Step Breakdown

Data Exploration and Preparation

The project started by exploring the NHANES dataset to identify key health indicators that might be related to depression. Variables such as Age, BMI, and dietary habits were selected based on their relevance to mental health. This initial exploration involved visualizing data distributions and identifying potential issues, such as class imbalance, that could affect the analysis.

The NHANES dataset was preprocessed to address issues like data imbalance, where the "not depressed" category was significantly larger than the "depressed" category. Techniques such as oversampling the minority class were considered to ensure a balanced dataset for analysis.

Logistic Regression Analysis

The first analytical step involved building a logistic regression model to predict depression based on the selected health indicators. The dataset was split into training (75%) and testing (25%) sets to evaluate model performance. Cross-validation and bootstrapping techniques were applied to enhance the model's robustness.

The logistic regression models were iteratively refined, but challenges such as high rates of false positives and false negatives highlighted the complexity of predicting depression. Despite various adjustments, the accuracy remained moderate, prompting further exploration.

Dimensionality Reduction with PCA

To simplify the complex dataset and highlight key variables, Principal Component Analysis (PCA) was employed. PCA reduced the dimensionality of the data while retaining the most significant sources of variance, making it easier to identify patterns and relationships within the dataset.

The results from PCA were visualized using scatter plots, which revealed significant overlap among the clusters. This indicated that while some patterns were present, the data's complexity might require additional variables or more sophisticated methods for clearer insights.

Clustering with K-means

K-means clustering was applied to segment the population into subgroups based on the selected health indicators. The silhouette analysis was conducted to determine the optimal number of clusters, with three clusters providing the most coherent grouping.

Despite the clustering efforts, the results suggested only subtle differences between groups, reinforcing the notion that depression is influenced by a complex interplay of factors. The cluster profiles were analyzed to uncover characteristics that might differentiate the groups, such as age and dietary patterns.

Classification with Tree-Based Methods

Tree-based methods, specifically classification trees, were used to further analyze the relationships between health indicators and depression. The initial tree model struggled with the class imbalance, predicting only the "not depressed" category.

To address this, the upSample function from the caret library was employed, which balanced the data by sampling with replacement. The revised tree model provided better classification results, particularly highlighting BMI and frozen meals/pizzas as significant predictors.

Code

The R code for this entire project can be found on the Github Repository under WorkingFinalCode415.Rmd

Visuals/Report

The full report that includes a deeper dive into the project, as well as all of the visualizations can be found here

Summary

This project has been instrumental in enhancing both my analytical and technical skills. It represented my first comprehensive application of advanced statistical methods like logistic regression, PCA, K-means clustering, and tree-based models to explore a complex health dataset. While the challenges of predicting depression proved difficult, the experience deepened my understanding of how to approach multifaceted problems in data science. Moreover, I gained valuable insights into handling class imbalance, dimensionality reduction, and model refinement, all of which are critical in building effective predictive models. This project has not only strengthened my ability to analyze health data but also equipped me with practical skills that will be invaluable in future data science endeavors.
