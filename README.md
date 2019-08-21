## PREDICTING CONVERSION FROM GOOGLE MERCHANDISE STORE
This project aims to build a machine learning algorithm for predicting whether customers visiting Google's Merchandise Store will make a purchase in the next 7 days.

Contributed by: Lim Si Ling Evelyn, Lee Meng Yong, Jiang Nan, Desmond Ho<br>
Pls contact desmondhw@gmail.com for any questions.

**Data**:<br>
Google Merchandise Store clickstream data from Google Bigquery from 1 November 2016 to 30 July 2017.<br><br>
Dataset was extracted by incorporating SQL queries into the Python codes in Google Colab - See **Data_Extraction_and_Exploratory_Data_Analysis.ipynb** under codes folder.
https://bigquery.cloud.google.com/table/bigquery-public-data:google_analytics_sample.ga_sessions_20170801

 
Note: Target variable (transaction) is highly imbalanced with only 3.9% of the non-bounce sessions making a transaction.

**Performance Metric:** <br>
F2-score. F2-score considers both precision and recall in the measurement, but implicit computation will give a higher weightage to recall measure, i.e. the ability for the model to be able to capture as many potential customers as possible. 

**Models:**<br>
Random Forest using data without LDA, PCA obtained the highest F2-score for the test data out of all the combinations tried.<br><br>
Best model
* Models without LDA _ PCA.ipynb<br>

Other models
* Models with LDA.ipynb
* Models with PCA.ipynb
* Models without LDA _ PCA with undersampling.ipynb


**Report:**<br>
Our full report can be found in: 'Project Report - Applied Machine Learning.docx'

**Requirements:** <br>

* Python 3.7 <br>
* Jupyter Notebook

**Python Libraries Required:**<br>

* datetime<br>
* numpy<br>
* pandas<br>
* scikit-learn<br>
* matplotlib.pyplot<br>
* seaborn<br>
* dmatrices<br>
* statsmodels<br>
* lightgbm<br>
* pickle<br>


Python libraries above can be installed via `pip`. Note that we only tested with the versions above, newer versions might not work.
