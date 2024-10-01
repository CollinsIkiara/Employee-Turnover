# Employee Turnover Analysis and Prediction  
by [Collins Ikiara], 2024  

## Project Title  
Employee Turnover Analysis and Prediction  

## Project Description  
This project analyzes employee turnover data to understand the factors that contribute to employees leaving an organization. Using exploratory data analysis (EDA) and machine learning models, the notebook investigates key factors such as employee satisfaction, salary, workload, and other variables that may influence turnover. The goal is to predict which employees are likely to leave, enabling companies to take proactive measures to retain talent.

## Installation Instructions
1. Clone this repository:
   ```
   git clone https://github.com/CollinsIkiara/employee-turnover.git  
   cd employee-turnover  
   ```
2. Create a virtual environment (optional but recommended):
   ```
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```
3. Install required libraries:
   ```
   pip install -r requirements.txt
   ```
4. Launch Jupyter Notebook:
   ```
   jupyter notebook 'Employee Turnover Analysis.ipynb'
   ```

## Usage  
1. Open the `Employee Turnover Analysis.ipynb` notebook in Jupyter.  
2. Run the cells in order to perform the data analysis, model training, and evaluation steps.  
   The notebook includes data preprocessing, feature engineering, and the application of machine learning models such as Random Forest to 
   predict employee turnover.

## Datasets  
The dataset used for this analysis includes various features such as:  
- **Department**: The department the employee belongs to. (categorical)  
- **Promoted**: 1 if the employee was promoted in the previous 24 months, 0 otherwise. (integer)  
- **Review**: The composite score the employee received in their last evaluation. (decimal/float)  
- **Projects**: How many projects the employee is involved in. (integer)  
- **Salary**: For confidentiality reasons, salary comes in three tiers: low, medium, high. (categorical)  
- **Tenure**: How many years the employee has been at the company. (decimal/float)  
- **Satisfaction**: A measure of employee satisfaction from surveys. (decimal/float)  
- **Bonus**: 1 if the employee received a bonus in the previous 24 months, 0 otherwise. (integer)  
- **Avg_hrs_month**: The average hours the employee worked in a month. (decimal/float)  
- **Left(target variable)**: "yes" if the employee ended up leaving, "no" otherwise. (categorical)

(Source: [Kaggle](https://www.kaggle.com/datasets/marikastewart/employee-turnover?resource=download))

## Workflow
The analysis process follows these key steps:

### Exploratory Data Analysis (EDA):
- Inspect the data for missing values, inconsistencies, and outliers.
- Visualize key distributions in the data such as employee satisfaction, salary distribution, etc.

### Data Preprocessing:
- Encode categorical variables, such as department or salary level, to make them suitable for machine learning models.
- Scale numeric features to normalize the data.

### Feature Engineering:
- Select important features such as job satisfaction, tenure, and performance evaluations.
- Create new features that may contribute to the model’s performance, such as interaction terms or derived metrics (review_zscore, 
  satisfaction_zscore etc.).

### Model Selection and Training:
- Apply machine learning models, like the Random Forest, to predict employee turnover.
- Train the model on a portion of the dataset and validate them on the remaining data.

### Model Evaluation:
- Evaluate the performance of each model using accuracy, precision, recall, and F1-score.
- Perform hyperparameter tuning to improve model performance where necessary.

### Prediction:
- Use the best-performing model to predict which employees are at risk of leaving the organization.


## Results  
The analysis identified significant factors contributing to employee turnover, such as job satisfaction and salary.  
The machine learning models used in this project achieved accurate predictions, with the most successful model being evaluated using metrics like accuracy, precision, recall, and F1-score.  
Insights from this analysis can help companies improve employee retention strategies by focusing on key factors affecting turnover.

## Contributors
- [Collins Ikiara](https://github.com/CollinsIkiara)

## License
This project is licensed under the CC0: Public Domain License - see the [LICENSE](LICENSE) file for details.

## Conclusion  
This project highlights how data analysis and predictive modeling can be used to understand employee turnover. By identifying the key drivers of turnover, companies can make data-driven decisions to improve employee retention and overall job satisfaction.

## Future Improvements  
- **Inclusion of Additional Features**: Adding more detailed employee data such as engagement scores or external factors (e.g., job market conditions) to enhance the prediction model.  
- **Real-Time Monitoring**: Incorporating real-time data to monitor employee turnover trends and predict future turnover more accurately.  
- **Deployment**: Developing a web-based dashboard to allow HR professionals to interact with the data and predictions.
