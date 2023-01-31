<div id="bootcamp"><img style="display: none;" src="https://static.bc-edx.com/data/dl-1-1/m20/lms/img/banner.jpg" alt="lesson banner" />

### Background

You are on the data science team of a medical research company that’s interested in finding better ways to predict myopia, or nearsightedness. Your team has tried&mdash;and failed&mdash;to improve their classification model when training on the whole dataset. However, they believe that there might be distinct groups of patients that would be better to analyze separately. So, your supervisor has asked you to explore this possibility by using unsupervised learning.

You have been provided with raw data, so you’ll first need to process it to fit the machine learning models. You will use several clustering algorithms to explore whether the patients can be placed into distinct groups. Then, you’ll create a visualization to share your findings with your team and other key stakeholders.

### Instructions

This activity is broken down into four parts:

* Part 1: Prepare the Data.

* Part 2: Apply Dimensionality Reduction.

* Part 3: Perform a Cluster Analysis with K-means.

* Part 4: Make a Recommendation.

#### Part 1: Prepared the Data

1. Read `myopia.csv` into a Pandas DataFrame.

2. Removed the "MYOPIC" column from the dataset.

3. Standardized the dataset so that columns that contained larger values did not influence the outcome more than columns with smaller values.

#### Part 2: Applied Dimensionality Reduction

1. Performed dimensionality reduction with PCA.

2. Further reduced the dataset dimensions with t-SNE and visually inspected the results. To do this, I ran t-SNE on the principal components, which was the output of the PCA transformation.

3. Created a scatter plot of the t-SNE output.

![scatter_plot](https://github.com/Kaludii/unsupervised-machine-learning-challenge/blob/main/Images/scatter_plot.png?raw=true)

#### Part 3: Performed a Cluster Analysis with K-means

Created an elbow plot to identify the best number of clusters. Made sure to do the following:

* Used a `for` loop to determine the inertia for each `k` between 1 through 10.

* Determined where the elbow of the plot was, and at which value of `k` it appeared.

![cluster_analysis_kmeans](https://github.com/Kaludii/unsupervised-machine-learning-challenge/blob/main/Images/cluster_analysis_kmeans.png?raw=true)

#### Part 4: Made a Recommendation

Based on the findings, wrote up a brief (one or two sentences) recommendation for my supervisor in your Jupyter Notebook.

### References

Reduced dataset from [Orinda Longitudinal Study of Myopia conducted by the US National Eye Institute](https://clinicaltrials.gov/ct2/show/NCT00000169)
