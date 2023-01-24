# HOUSING-PRICE-PREDICTION

--------Read Me-------

Data source：
a. Perth housing price data: https://www.kaggle.com/syuzai/perth-house-prices
b. transportation data: https://catalogue.data.wa.gov.au/dataset/public-transport-authority-stops-bus-stops

1. Time_series_analysis.ipynb
    Function: analyze the whole data trend. For example, the count of monthly mean price, the trend of monthly mean price
    Data: all_perth_310121.csv from a)

2. Data cleaning.ipynb
    Function: Add three non-housing data in. For example: transport data, school rank data, cemetery data
    Data: all_perth_310121.csv from a), bus.csv from b), cemetery.csv data collected by ourselves

3. Data-preprocessing.ipynb
    Function: Exploratory data analysis and visualization, including heat map and calculating VIF
    Data: perth_pro.csv from 2.

4. Price_model.ipynb
    Function: build LSTM and GRU model to predict the Dec.2020 monthly mean price and preserve
    Data: perth_pro.csv from 2.

4.5 402——param.ipynb
    Function: find the best hyper-parameters. Better to use Colab to see the visualization. 
    Here is the Colab link: https://colab.research.google.com/drive/1lc9tS3FaPtsVbMhVNncIXsUnHhLLUen-?usp=sharing
    To see the visualization, click HPARAM in the middle of the top; click PARALLEL COORDINATES VIEW in the middle of
    the second line; click the line to see the corresponding parameters
    Data: perth_pro.csv fro 2.
    
5. Adjusted_model.ipynb
    Function: build four models including Random Forest, KNN, Gradient Boosting and XGBoost to finally predict housing price. Test with the application data
    Data: perth_with_mean.csv from 4.
