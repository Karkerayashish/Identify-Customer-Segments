# Identify Customer Segments project

## 1. Installation
I use python 3.5 to create this project and the libraries I used are:
 - Pandas
 - Numpy
 - Matplotlib
 - Seaborn
 - Scikit-Learn


## 2. Project Motivation

In this project, I work with real-life data provided to us by our Bertelsmann partners AZ Direct and Arvato Finance Solution. The data here concerns a company that performs mail-order sales in Germany. Their main question of interest is to identify facets of the population that are most likely to be purchasers of their products for a mailout campaign. My job as a data scientist is to use unsupervised learning techniques to organize the general population into clusters, then use those clusters to see which of them comprise the main user base for the company. Prior to applying the machine learning methods,  I also need to assess and clean the data in order to convert the data into a usable form.

## 3. File Descriptions
  - Identify_Customer_Segments.ipynb
      - This is the file that I used to analyze the azdias the questions. I use mechine learning to analyze the dataset.
      - Use the k-means method to cluster the demographic data into groups.
      - Apply the techniques and models that you fit on the demographic data to the customers data: data cleaning, feature scaling, PCA, and k-means clustering. Compare the distribution of people by cluster for the customer data to that of the general population.
  - Identify_Customer_Segments.html
      - It is html format of above ipynb

  - The .csv files
       - Udacity_AZDIAS_Subset.csv: Demographics data for the general population of Germany; 891211 persons (rows) x 85 features (columns).
       - Udacity_CUSTOMERS_Subset.csv: Demographics data for customers of a mail-order company; 191652 persons (rows) x 85 features (columns).
       - Data_Dictionary.md: Detailed information file about the features in the provided datasets.
       - AZDIAS_Feature_Summary.csv: Summary of feature attributes for demographics data; 85 features (rows) x 4 columns


## 4. Summary of the results of the analysis

I use elbow method to select 8 clusters and analyze the dataset via PCA method and find out 50 principle components based on 8 clusters. I calculate the percentage on each cluster id for the customer dataset and general dataset. and then get the ratio of customer to general population. The value 1 is threshold. If above 1.0 the cluster may be target audience of mail-order. If the ratio with below 1.0 is not. Since used 8 clusters, the customer data for some of the clusters had low population and even though they were below 1.0 threshold. I draw a chart and I find that the most overrepresented cluster id is 6 and underrepresented cluster id is 4 among 8 clusters. I select them to do further analysis.

## 5. Licensing, Author, Acknowledgements
 - I make this project to help people understand mailout company customers. If it is useful, I will be glad to hear from you! Feel free to use  this and mention me so I can take a look at your work.
 - Thanks for AZ Direct and Arvato Finance's dataset!
