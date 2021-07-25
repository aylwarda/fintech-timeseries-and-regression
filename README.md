# fintech-timeseries-and-regression
This project is the start of Machine Learning as part of my FinTech homework, incorporating some time-series forecasting and linear regression modelling.  I use [statsmodels](https://www.statsmodels.org/stable/index.html), [ski-kit learn](https://scikit-learn.org/stable/) (as well as the now staple numpy, Pandas, Matplotlib) for modelling, all within Jupyter Labs Notebooks; my work builds on coursework that I am involved in.

---
## Instructions / Intro
Within this Project, there are two Jupyter Notebooks.
 - Time-series Analysis (`time_series_analysis.ipynb`)
 - Regression Analysis (`regression_analysis.ipynb`)

To run through either Notebook, execute the one you are interested in, and follow the analysis and conclusions for each.  These are not particularly mind-blowing in terms of visualisation but are a look into the start of Machine Learning in fairly simple terms.

The financial data used in this Project is currency pricing data for Canadian Dollar / Japanese Yen (CAD/JPY) and found in `./Resources/cad_jpy.csv`

---
## Time-series Analysis
This Notebook explores the decomposition of the CAD/JPY returns and seeks to understand any patterns, short-term or long-term.  This is done by plotting returns over time, making trending data stationary and exploring volatility.  Forecasting both returns as well as volatility is attempted and judgments made on those forecasts in the use of differing models and their comparitive results.

**Models Used**
- Decomposition
  - Hodrick-Prescott Filter
- Forecasting Returns
  - ARMA Model
  - ARIMA Model
- Forecasting Volatility
  - GARCH Model


## Regression Analysis
This Notebook explores the CAD/JPY data a little further using linear regression.  The data is split into different samples, ready to "train" the linear regression model using Machine Learning's train-test split. This is essentially a splitting of the data into samples used for training the model and once "trained", is tested using the remainder of the data, i.e. the test sample.

To determine the veracity of the linear regression model, Machine Learning's model-fit-predict is also used, in that, one determines the model, then one fits the model to the data and finally one predicts.  

The performance of the model is tested using RMSE (root mean squared error) for both the training set as well as the testing data samples and then the performance compared.

---
## Acknowledgements
### Sources
- Sci-kit Learn and statsmodels as referenced in the introduction.
- Learnt a little formatting trick or two from these padding examples at [stackabuse.com](https://stackabuse.com/padding-strings-in-python)
- Data source provided by Trinity College as part of course work.
