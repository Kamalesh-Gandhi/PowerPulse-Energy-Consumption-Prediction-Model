# PowerPulse: Household Energy Usage Forecast

## Project Overview
PowerPulse is a predictive analytics project focused on forecasting household energy consumption using historical data. The primary objective is to assist households in optimizing energy consumption patterns and enable energy providers to improve load forecasting and anomaly detection. The project applies advanced machine learning techniques, including data preprocessing, feature engineering, and multiple regression models, to build an accurate energy prediction system.

By combining statistical analysis with machine learning models, PowerPulse aims to generate actionable insights for smarter energy management and sustainable resource utilization.

## Dataset Information
**Dataset:** Time-series data of electric power consumption in a single household collected at one-minute intervals over four years. It includes detailed measurements of electrical quantities and sub-metering values.  
**Data Type:** Multivariate, Time-Series Data  

## Technical Stack & Tools
- **Languages:** Python  
- **Libraries:** Scikit-learn, Pandas, NumPy, Matplotlib, Seaborn, XGBoost, SciPy, TensorFlow/Keras  
- **Models:** Linear Regression,  Random Forest, Gradient Boosting, Neural Networks (MLP), XGBoost, K-Nearest Neighbors (KNN)

## Approach
1. **Data Understanding and Exploration**
   - Loaded and explored the dataset to understand structure, data types, and missing values.
2. **Data Preprocessing**
   - Handled missing values and converted data types where needed.  
   - Detected and treated outliers using statistical methods such as Z-score and IQR.  
   - Removed duplicates and managed placeholder values.  
3. **Feature Engineering**
   - Generated time-based features (`Hour`, `DayOfWeek`, `Month`, `IsWeekend`).  
   - Created rolling averages for 10-minute, 1-hour, and 24-hour power usage.  
   - Introduced custom features like `Power_Anomaly_Flag` to detect deviations from expected consumption.  
4. **Exploratory Data Analysis (EDA)**
   - Analyzed trends and seasonal patterns in energy usage.  
   - Visualized feature correlations and distributions.  
5. **Model Selection and Training**
   - Split the dataset into training and testing sets.  
   - Trained multiple machine learning models on 30% of the dataset (~600,000 samples).  
   - Applied regression models including Linear Regression, Random Forest, Gradient Boosting, Neural Network (MLP), and XGBoost.  
6. **Evaluation**
   - Evaluated models using error metrics: MAE, RMSE, and R² Score.
   ![image](https://github.com/user-attachments/assets/3cba82f8-c21e-426c-ba3f-66d5e1b09436)
     
   - Compared model performances and selected the best model for deployment.

## Technologies Used
| Technology   | Purpose                                                       |
|--------------|---------------------------------------------------------------|
| Python       | Core programming language for data analysis and modeling       |
| Pandas       | Data manipulation and preparation                             |
| NumPy        | Numerical computing and array operations                       |
| Matplotlib   | Visualization of trends and patterns                           |
| Seaborn      | Enhanced visualization with detailed plots                     |
| Scikit-learn | Machine learning model development and evaluation              |
| XGBoost      | High-performance gradient boosting models                      |
| SciPy        | Statistical analysis                                           |
| TensorFlow/Keras | Neural network model implementation                        |

## Installation & Setup
To run this project, install the necessary dependencies using the following command:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost scipy ucimlrepo
