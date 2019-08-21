![1_UotPZNT_c_BjECWSx00pPw](https://user-images.githubusercontent.com/34176396/63445590-3cac9980-c46b-11e9-9b07-e34c9801a98f.png)
## PREDICTING CONVERSION FROM GOOGLE MERCHANDISE STORE
This project aims to build a machine learning algorithm for predicting whether customers visiting Google's Merchandise Store will make a purchase in the next 7 days.

Contributed by: Lim Si Ling Evelyn, Lee Meng Yong, Jiang Nan, Desmond Ho<br>
Pls contact desmondhw@gmail.com for any questions.

**Data**:<br>
Google Merchandise Store clickstream data from Google Bigquery from 1 November 2016 to 30 July 2017.<br><br>
Dataset was extracted by incorporating SQL queries into the Python codes in Google Colab - See **Data_Extraction_and_Exploratory_Data_Analysis.ipynb** under codes folder.
https://bigquery.cloud.google.com/table/bigquery-public-data:google_analytics_sample.ga_sessions_20170801

**Training Dataset**:<br>
Data\test_dataset.csv<br>
**Testing Dataset**:<br>
Data\train_validation_dataset.csv

Note: Target variable (transaction) is highly imbalanced with only 3.9% of the non-bounce sessions making a transaction.

**Performance Metric:** <br>
F2-score. F2-score considers both precision and recall in the measurement, but implicit computation will give a higher weightage to recall measure, i.e. the ability for the model to be able to capture as many potential customers as possible. 

**Models:**<br>
Random Forest using data w/o any LDA feature engineering and w/o PCA obtained the highest F2-score for the test data out of all the combinations tried.<br><br>
Best model
* Codes\Models without LDA _ PCA.ipynb<br>

Other models
* Codes\Models with LDA.ipynb
* Codes\Models with PCA.ipynb
* Codes\Models without LDA _ PCA with undersampling.ipynb

Tableau:<br>
* Codes\outliers.twbx - This visual demonstrated why Anomaly Detection models didn't work well due to the minority class(purchase) not appearing as anomalies, but clustered with the majority.

![Screenshot 2019-08-21 at 22 55 45](https://user-images.githubusercontent.com/34176396/63444603-8300f900-c469-11e9-946f-0519ca38e7ab.png)


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


Python libraries above can be installed via `pip`. Note that we only tested with the versions above, newer versions might not work.
