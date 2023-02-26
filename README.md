# Whoop-Data-Analysis
Collection of visualizations and decision tree to classify my fitness scores
# Project Overview
* Exported one year worth of my fitness data from Whoop 4.0 (wearable fitness tracker). 
* Engineered features of categories of recovery score based on what I have felt over the year. 
* Used visualzation tools to analyze data. 
* Optimized decision tree to learn the rules of the process to a certain recovery score. 
# Code & Resources Used
Python Version: 3.9.12 | Tableau Public
* Python Packages: pandas, numpy, sklearn, matplotlib, seaborn
* Prunning Decision Tree: https://towardsdatascience.com/decision-tree-build-prune-and-visualize-it-using-python-12ceee9af752
# Data Collection
Whoop moblie app provides a data export function which Whoop sends a CSV file over personal email. 
* Detail information on exporting data: https://support.whoop.com/APP_FEATURES__COACHING/Understanding_Your_WHOOP_Features/How_to_Export_Your_Data
# Data Cleaning
After collecting the data I have made the following changes: 
* Deleted useless columns 
* Dropped all null values
* Changed all dates into datetime data type
* Made few categorical and boolean columns regarding recovery score and date
# EDA
I have visualized through Tableau Public. Here are some of the foundings: 

<img width="292" alt="Screen Shot 2023-02-23 at 1 35 11 PM" src="https://user-images.githubusercontent.com/118776460/221281977-3fc65d9f-bcd9-4be7-a50e-044126c71500.png">
<img width="713" alt="Screen Shot 2023-02-24 at 11 26 58 AM" src="https://user-images.githubusercontent.com/118776460/221281999-62082404-545d-4c05-b397-757efac2d7b4.png">
<img width="716" alt="Screen Shot 2023-02-24 at 11 26 32 AM" src="https://user-images.githubusercontent.com/118776460/221282009-7ec96545-2f3f-469e-b731-5bab1d5466c9.png">

# Model Building
I have built two decision tree to see the process of rules that are associated with the specified recovery score which are over 40% and over 90%.
I also split the data into train and test sets with a test size of 33%.
# Model Performance
I have used a loop to find the best criterion and max depth for the two model. 
* Over 40% Model: 0.94
* Over 90% Model: 0.87
