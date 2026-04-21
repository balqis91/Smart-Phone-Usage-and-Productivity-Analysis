# Smart-Phone-Usage-and-Productivity-Analysis
This project analyses how smartphone usage behaviour impacts work productivity. The analysis was carried out using Python, focusing on data cleaning, exploration, visualisation, and predictive modelling.
# Smartphone Usage & Productivity Analysis

## Project Overview
This project investigates how smartphone usage behaviour influences work productivity. The analysis was carried out using Python, focusing on understanding the dataset, exploring patterns, and building a simple predictive model. The dataset was imported into a pandas DataFrame, which served as the primary structure for data manipulation and analysis. Essential libraries such as Pandas (for data handling), Matplotlib and Seaborn (for visualisation), and Scikit-learn (for predictive modelling) were also imported.


## Dataset

The dataset contains information on users’ daily habits, including phone usage, social media activity, sleep, stress levels, and productivity scores. It also includes demographic variables such as gender, occupation, and device type.

---

## Data Cleaning & Preparation

The analysis began by exploring the dataset to understand its structure and quality.

The first step was to view the dataset using `.head()` to understand how the data is organised and what each column represents. This provided a quick overview of the variables and their format.

Next, the structure of the dataset was examined using `.info()` to check the data types of each column and confirm whether any conversions were required.

The dataset was then checked for missing values and duplicate records. No significant missing values were identified, and duplicate rows were removed to ensure the dataset was clean and reliable for analysis.

Column names were also reviewed and formatted consistently to make them easier to reference throughout the analysis.

*The image below shows the first five rows of the dataset:*
<img width="1078" height="317" alt="image" src="https://github.com/user-attachments/assets/888b59bb-b122-403c-be05-9f7a23986d3a" />
)

*The image below shows the dataset structure and data types:*
<img width="558" height="562" alt="image" src="https://github.com/user-attachments/assets/e4a08c62-47be-45d8-95ab-33fad8f85e70" />


---

## Exploratory Data Analysis (EDA)

### Distribution of Numerical Variables

To understand how the data is distributed, histograms were created for all numerical variables. This helped identify patterns such as skewness, spread, and potential outliers.

For example, variables like daily phone usage and productivity scores were analysed to observe how values are distributed across users.

*The image below shows some of the distribution of numerical variables:*
<img width="917" height="701" alt="image" src="https://github.com/user-attachments/assets/1f4aec0e-baf2-48cd-9e58-7b137e1074f9" />
)
<img width="943" height="503" alt="image" src="https://github.com/user-attachments/assets/745acac4-00fc-4b27-8022-9ed50dc21b27" />
<img width="937" height="488" alt="image" src="https://github.com/user-attachments/assets/ccc5fb0b-bfd1-48e5-a101-626b8d3fa825" />


---

### Analysis of Categorical Variables

Categorical variables such as Gender, Occupation, and Device Type were analysed using count plots. This helped to understand how the data is distributed across different groups.

This step provided insight into the composition of the dataset and ensured there was a balanced representation of categories.

*The image below shows the categorical distributions codes and outputs:*
<img width="1111" height="605" alt="image" src="https://github.com/user-attachments/assets/63e602a7-4763-4ab0-ba4d-17f8ee907222" />
<img width="1060" height="260" alt="image" src="https://github.com/user-attachments/assets/0cd93a51-0ec0-4211-a0ec-0e843fb722ae" />
<img width="1041" height="577" alt="image" src="https://github.com/user-attachments/assets/cb56669c-31f4-49d8-9893-1c74626f6a7b" />
<img width="1071" height="582" alt="image" src="https://github.com/user-attachments/assets/c5e13a45-26f8-4a99-ab72-4e93ee25e4f8" />





---

## Correlation Analysis

A correlation matrix was generated to examine relationships between numerical variables.

This step was important to identify which variables have the strongest relationship with productivity. Positive correlations indicate variables that increase productivity, while negative correlations indicate variables that reduce productivity.

*The image below shows the correlation analysis and heatmap:*
<img width="1057" height="368" alt="image" src="https://github.com/user-attachments/assets/f959c304-979b-4cde-99a7-b9179ad6c2c1" />
<img width="1118" height="707" alt="image" src="https://github.com/user-attachments/assets/727ae8cb-976a-4d89-a3d9-e7d800888f82" />



---

## Relationship Analysis

To further explore relationships, scatter plots were created between key variables and productivity.

These included:

* Daily phone usage vs productivity
* Social media usage vs productivity
* Sleep hours vs productivity
* Stress level vs productivity

This helped to visually confirm trends observed in the correlation analysis.

*The image below shows the relationship between variables and productivity:*
<img width="912" height="562" alt="image" src="https://github.com/user-attachments/assets/46f42cde-82bf-4c7a-b392-4fefe3dc269b" />
<img width="932" height="578" alt="image" src="https://github.com/user-attachments/assets/94b2c408-2537-4529-8ae9-1d0adf5f1284" />
<img width="897" height="588" alt="image" src="https://github.com/user-attachments/assets/c0262e36-44c6-4757-a9fe-136ad366ef8a" />
<img width="868" height="570" alt="image" src="https://github.com/user-attachments/assets/8ecdf3e0-e910-4821-b21f-ddf424d5a263" />



---

## Feature Engineering

A new variable called **Usage_Level** was created by categorising daily phone usage into three groups: Low, Medium, and High.

This made it easier to compare how different levels of phone usage affect productivity.

Box plots were then used to compare productivity, stress, and sleep across these usage levels.

*The image below shows productivity across usage levels:*
<img width="667" height="292" alt="image" src="https://github.com/user-attachments/assets/1abd5697-691a-4b3a-a548-f7600963fbc2" />
)
<img width="932" height="576" alt="image" src="https://github.com/user-attachments/assets/c6bfdc22-05c1-47b1-95ab-c24fa1fe7aea" />
<img width="697" height="715" alt="image" src="https://github.com/user-attachments/assets/485d71de-242f-41ba-9bc2-7f335bea7ae5" />
<img width="885" height="677" alt="image" src="https://github.com/user-attachments/assets/eee87c2a-e8f7-47c9-8893-d79a499cf6a3" />



---


---

## Predictive Modelling

A Linear Regression model was developed to predict productivity based on behavioural factors.

The features used in the model included:

* Daily phone usage
* Social media usage
* Sleep hours
* Stress level
* App usage count
* Caffeine intake

The dataset was split into training and testing sets, and the model was trained on the training data before being evaluated on unseen data.

---

## Model Evaluation

The performance of the model was evaluated using R² Score, Mean Absolute Error (MAE), and Root Mean Squared Error (RMSE).

These metrics were used to assess how accurately the model predicts productivity.

📸 *The image below shows the model evaluation results:*
<img width="642" height="627" alt="image" src="https://github.com/user-attachments/assets/c010120b-e35d-4241-af36-cda222de3843" />
<img width="562" height="283" alt="image" src="https://github.com/user-attachments/assets/aac4d7da-2182-4677-9f35-0b4d1481d653" />
<img width="361" height="290" alt="image" src="https://github.com/user-attachments/assets/ef7ad12d-12fb-4e66-8f88-980faee65651" />



---

## 📊 Model Visualisation

The model results were visualised using:

* A scatter plot comparing actual vs predicted productivity
* A bar chart showing feature importance (model coefficients)

This helped to understand how each variable influences productivity.

📸 *The image below shows the model predictions:*
<img width="608" height="308" alt="image" src="https://github.com/user-attachments/assets/d96939ac-1c18-40c8-85a0-d107df560041" />


📸 *The image below shows feature importance:*
<img width="943" height="565" alt="image" src="https://github.com/user-attachments/assets/74c3b2b6-556b-4b3c-9c1f-7a6df87bb0fa" />
)
<img width="1052" height="580" alt="image" src="https://github.com/user-attachments/assets/5e74bb55-ae7f-45b3-8f95-9574e52c716a" />

---

## Key Insights

From the analysis, several important insights were identified:

* Higher smartphone usage is associated with lower productivity
* Increased social media usage negatively impacts productivity
* Better sleep is linked to higher productivity
* Higher stress levels reduce productivity
* Moderate phone usage provides a balance between engagement and productivity

---

## Conclusion

This project demonstrates how behavioural data can be analysed to uncover meaningful patterns and relationships. It highlights the impact of lifestyle and technology usage on productivity and shows how data analysis can support better decision-making.

---

## Tools Used

Python, Pandas, Matplotlib, Seaborn, Scikit-learn

---

## Author

Balikisu Ajoke (AJ) Oniyide
Data Analyst
