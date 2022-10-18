# Credit-Card-Fraud-Analysis
  data
    card_transdata.csv
      url: https://www.kaggle.com/datasets/dhanushnarayananr/credit-card-fraud?resource=download
  method
    The data ended up being synthetic and without a source, so steps were taken to evaluate it from 3 angles:
      1) Modeling the data as is (after cleaning it).
      2) Re-weighing the data.
      3) Oversampling the data.
    The data being evaluated was a collection of fradulent credit card transactions, and my goal with modeling
    the data was to isolate the leading correlating factor to a fradulent transaction. The main recommended 
    machine-learning model was Catboost but I also used XGBoost for its straightforward implementation of 
    scale_pos_weight for the re-weighing portion.
  data cleaning
    The data was essentially spotless on arrival. All column names were easily readable, there were no instances
    of multiple differing data types per feature, and there were no null values.
  EDA
    There were just a few outliers. Eight to be specific out of one million.
  machine learning
    Per a quick Google search, Catboost came back as a well-used model for this type of evaluation. I employed it
    and XGBoost to run 3 models (as outlined in my method above).
  predictions and results
    I didn't have any predictions going in. Fradulent transactions have been a focus for a while now, so I just 
    wanted to see what was leading to it more than anything else. In 2/3 of the models, the ratio_to_median_
    purchase_price was the common anchor.
  notebooks
    Data Cleaning and EDA
    Pre-processing and Modeling
 
