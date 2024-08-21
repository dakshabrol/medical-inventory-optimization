# 🏥 Pharma Forecast: Optimizing Medical Inventory

⚙️ **Tech Stack** : Python, MySQL <br>
📊 **Presentation** : PowerPoint <br>

## 📂 **Project Overview**

Unveil the power of time series forecasting to revolutionize pharmaceutical inventory management. This project showcases a comprehensive pipeline, divided into three captivating phases:

1. 🧹 Data Preparation: Feature engineering and cleaning
2. 🔍 Exploratory Analysis: Unraveling time-series insights
3. 🔮 Forecasting: Predicting future demand

<br>

---

## 📂 **Task 1 - Scope & Context**

### **Setting the Stage**

Developing a cutting-edge pharmaceutical forecasting model aims to mitigate the potential occurrence of dreaded drug shortages. By collecting historical sales data and meticulously analyzing it, we identify patterns and trends in drug demand. Based on this data-driven analysis, we have crafted a forecasting model that accurately predicts the demand for essential medical supplies. The project involves gathering data on inventory levels, usage patterns, and other relevant factors, which are then analyzed to uncover trends and patterns in supply and demand.

**Business Challenges:** 
- 🏪 Dwindling drug stocks
- 🚪 High bounce rates
  
**Business Goals:** 
- 📉 Minimize drug shortages
- 📈 Maximize drug availability, customer satisfaction, and profits

**Data Dictionary:** 
<br>

<p align="center">
  <kbd><img width="700" src="https://raw.githubusercontent.com/dakshabrol/medical-inventory-optimization/main/images/fig%2001%20-%20Data%20Dictionary.png"></kbd> <br>
  Figure 01 — Data Dictionary
</p>
<br>

---

## 📂 **Task 2 - Data Preprocessing**

### **Laying the Foundation**

Based on the problem and objective formal definition, the data sales transactions information system are cleaned, feature engineering approach was defined, and all data are transformed to monthly time series, consisting of aggregate sales among different classes of pharmaceutical drugs in monthly time periods.

## **Cleaning & Transforming**

### **Objectives**
- 🧹 Data Cleaning: Identifying errors, inconsistencies, and missing values
- 🔄 Data Transformation: Converting data into an appropriate format or scale for analysis or modeling
- 🛠️ Feature Engineering: Creating new relevant features or variables from existing data to enhance machine learning model performance<br>

8 data preprocessing methods were implemented:
1. Type Casting
2. Handling missing values
3. Removing duplicates
4. One-Hot encoding
5. Data manipulation

## **Descriptive Statistics**
1. 🏆 First Moment: Measure of Central Tendency
2. 📏 Second Moment: Measure of Dispersion
3. 🎢 Third Moment: Skewness
4. 📊 Forth Moment: Kurtosis

---

## 📂 Task 3 - Exploratory Data Analysis (EDA) 

### Uncovering Insights

After data preprocessing and descriptive statistics, our next step involves developing EDA to analyze the trends and patterns of the datasets.
 
### Objectives
- 🔍 Identify and analyze patterns, and trends within the data. 

### Results
#### 1. Data Distribution
<br>

<p align="center">
  <kbd><img width="500" src="https://raw.githubusercontent.com/dakshabrol/medical-inventory-optimization/main/images/fig%2002%20-%20Distribution%20of%20Data.png"></kbd> <br>
  Figure 02 — Distribution of Data. The Quantity data shows it is not normally distributed since the data is not falling within the straight line
</p>
<br>

#### 2. Data Transformation : Log Transformation
<br>

<p align="center">
  <kbd><img width="500" src="https://raw.githubusercontent.com/dakshabrol/medical-inventory-optimization/main/images/fig%2003%20-%20Log%20Transformation.png"></kbd> <br>
  Figure 03 — Log Transformation. After log transformation, the data is normally distributed.
</p>
<br>

#### 3. Histogram: Final Sales
<br>

<p align="center">
  <kbd><img width="500" src="https://raw.githubusercontent.com/dakshabrol/medical-inventory-optimization/main/images/fig%2004%20-%20Quantity%20of%20drugs%20sold%20by%20month%201.png"></kbd> <br>
  Figure 04 — Quantity of drugs sold by month
</p>
<br>

- Max. = 39490
- Right-skewed
- Most of transactions involve lower sales amounts, but there are a few instances with significantly higher sales amounts

#### 4. Bar Plot: Quantity of drugs sold by month
<br>

<p align="center">
  <kbd><img width="500" src="https://raw.githubusercontent.com/dakshabrol/medical-inventory-optimization/main/images/fig%2005%20-%20Quantity%20of%20drugs%20sold%20by%20month%202.png"></kbd> <br>
  Figure 05 — Quantity of drugs sold by month. The month of March, April, July, and September has highest quantity of medicines sold and it is approximately same.
</p>
<br>

#### 5. Trend in Quantity
<br>

<p align="center">
  <kbd><img width="500" src="https://raw.githubusercontent.com/dakshabrol/medical-inventory-optimization/main/images/fig%2006%20-%20Quantity%20Trend.png"></kbd> <br>
  Figure 06 — Quantity Trend. December has the highest quantity of medicines sold while February and June is the lowest.
</p>
<br>

#### 5. AutoEDA: D-Tale
<br>

<p align="center">
  <kbd><img width="600" src="https://raw.githubusercontent.com/dakshabrol/medical-inventory-optimization/main/images/fig%2007%20-%20AutoEDA%20using%20D-Tale.png"></kbd> <br>
  Figure 07 — AutoEDA using D-Tale.
</p>
<br>

---

## 📂 Task 4 - Forecasting Models

### Predicting the Future

Based on the analysis of the data, the project will develop forecasting models that predict the demand for medical supplies.
 
### Objectives
-  To accurately forecast future sales based on historical data, minimizing errors and improving predictive performance. 

### Model Building

1. 🔍 Select Models:
- 2 types of models being developed in this project: Random Forest Regression and Linear Regression.


2. 🏋️‍♀️ Train and Test Models:
- Split historical data into training and testing sets
- Train models on the training set using appropriate parameters
- Assess model performance on the testing set


3. 🔮 Generate Forecasts:
- Use trained models to predict future demand
- Compare predicted values with actual values from the testing set

  
4. 📊 Evaluation Metrics:
- Calculate common metrics to assess model accuracy
- Metrics for time series forecasting include:<br>
  i. Mean Squared Error (MSE)<br>
  ii. Root Mean Squared Error (RMSE)

### Results

#### 1. Holt-Winters Method
<br>

<p align="center">
  <kbd><img width="600" src="https://raw.githubusercontent.com/dakshabrol/medical-inventory-optimization/main/images/fig%2008%20-%20Forecast%20for%20the%20next%2012%20periods.png"></kbd> <br>
  Figure 08 — Forecast for the next 12 periods. 
</p>
<br>

- MAPE = nan
- RMSE = 5032.711977063249

#### 2. Random Forest Regression
<br>

<p align="center">
  <kbd><img width="600" src="https://raw.githubusercontent.com/dakshabrol/medical-inventory-optimization/main/images/fig%2009%20-%20Random%20Forest%20Regression%20Model.png"></kbd> <br>
  Figure 09 — Random Forest Regression Model
</p>
<br>

- MSE = 111.60992195041523

#### 3. Linear Regression
<br>

<p align="center">
  <kbd><img width="600" src="https://raw.githubusercontent.com/dakshabrol/medical-inventory-optimization/main/images/fig%2010%20-%20Linear%20Regression%20Model.png"></kbd> <br>
  Figure 10 — Linear Regression Model
</p>
<br>

- MSE = 159.57892788366377

#### Best Model

1. The Random Forest Model has a lower MSE (111.61) compared to the Linear Regression Model (159.58), indicating better prediction accuracy.
2. A lower MSE means the Random Forest Model's predictions are, on average, closer to the actual values, resulting in superior overall performance.
3. Random Forest can capture complex non-linear relationships in the data, which is crucial when dealing with diverse patterns in pharmaceutical sales and demand.
4. It is less sensitive to outliers compared to Linear Regression, leading to more reliable predictions.

---

#### Challenges Faced

1. 🔍 Predicting stock with return quantity when model implemented on quantity only
2. 🔒 Ensuring patient privacy while considering different health conditions and their impact on drug demand
3. 🧠 Limited knowledge in new drug development
4. 🏥 Aligning forecasting models with pharmaceutical regulations and patient privacy laws
5. 🔗 Integrating data with existing inventory systems is complex and time-consuming
7. 🌍 External factors like sudden market shifts or unexpected events (e.g., pandemics) can disrupt forecasting accuracy

#### Future Enhancements

**1. 🚀 Enhanced Forecasting Model:**
Continuously improve the pharmaceutical forecasting model by incorporating advanced machine learning techniques and considering additional factors like seasonal trends, public health events, and external influences on medicine demand.

**2. 🌐 Supply Chain Optimization:**
Collaborate with suppliers and distributors to optimize the entire supply chain. This might involve streamlining delivery routes, reducing lead times, and improving inventory management.

**3. 🧠 Machine Learning for Bounce Rate Reduction:**
Utilize machine learning to predict and mitigate factors causing high bounce rates in pharmacies, offering insights into optimizing store layouts and reducing product returns.
