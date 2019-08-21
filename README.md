## PREDICTING CONVERSION FROM GOOGLE MERCHANDISE STORE
This project aims to build a machine learning algorithm for predicting whether customers visiting Google's Merchandise Store will make a purchase in the next 7 days.

**Data**:<br>
Google Merchandise Store clickstream data from Google Bigquery from 1 November 2016 to 30 July 2017.<br><br>
Dataset was extracted by incorporating SQL queries into the Python codes in Google Colab - See **Data_Extraction_and_Exploratory_Data_Analysis.ipynb** under codes folder.
https://bigquery.cloud.google.com/table/bigquery-public-data:google_analytics_sample.ga_sessions_20170801

 
Note: Target variable (transaction) is highly imbalanced with only 3.9% of the non-bounce sessions making a transaction.


**Requirements:** <br>

Python 3.7 <br>
Jupyter Notebook

**Python Libraries Required:**<br>

datetime<br>
numpy<br>
pandas<br>
scikit-learn<br>
matplotlib.pyplot<br>
seaborn<br>


Python libraries above can be installed via `pip`. Note that we only tested with the versions above, newer version might not work.
