# HABERMAN_EDA
Overview
This project performs Exploratory Data Analysis (EDA) on the Haberman's Survival Dataset. The analysis aims to uncover patterns and insights related to the survival rates of patients who underwent surgery for breast cancer. Through detailed statistical analysis and data visualization, we explore how different factors influence patient survival outcomes.
Dataset Description
The Haberman's Survival Dataset contains cases from a study conducted between 1958 and 1970 at the University of Chicago's Billings Hospital on the survival of patients who had undergone surgery for breast cancer.
Features
The dataset consists of 306 instances with the following 4 attributes:
FeatureDescriptionData TypeAgeAge of the patient at the time of operationInteger (30-83 years)Operation YearYear of operation (year - 1900)Integer (58-69)Axillary NodesNumber of positive axillary nodes detectedInteger (0-52)Survival StatusSurvival status (Target Variable)Integer (1 or 2)
Target Variable

1: Patient survived 5 years or longer
2: Patient died within 5 years

Source
The dataset is publicly available from the UCI Machine Learning Repository.
Objectives
The main objectives of this exploratory data analysis are:

Understand the distribution of each feature in the dataset
Identify survival trends based on age, operation year, and number of axillary nodes
Analyze feature correlations and their impact on survival status
Detect outliers and handle missing values (if any)
Visualize relationships between variables using various plotting techniques
Extract meaningful insights that could inform predictive modeling or clinical decisions

Technologies Used
This project utilizes the following Python libraries and tools:

Python 3.x – Programming language
Jupyter Notebook – Interactive development environment
Pandas – Data manipulation and analysis
NumPy – Numerical computing
Matplotlib – Data visualization
Seaborn – Statistical data visualization
Warnings – Suppress unnecessary warnings

Steps in the Notebook
The Jupyter Notebook follows a structured approach to explore the Haberman dataset:
1. Importing Libraries

Load necessary Python libraries for data analysis and visualization

2. Loading and Inspecting Data

Import the dataset from CSV file
Display first/last few rows using head() and tail()
Check dataset shape, column names, and data types
Generate summary statistics using describe() and info()

3. Data Cleaning

Check for missing values
Identify and handle duplicate records
Detect outliers using statistical methods (IQR, box plots)
Validate data integrity and consistency

4. Univariate Analysis

Analyze individual features independently
Create histograms and density plots for continuous variables
Generate count plots for categorical variables
Study distribution patterns using box plots and violin plots

5. Bivariate Analysis

Examine relationships between pairs of variables
Create scatter plots to visualize correlations
Use pair plots to compare all features simultaneously
Analyze survival status against each feature

6. Multivariate Analysis

Explore interactions between multiple variables
Generate correlation heatmaps
Create grouped visualizations (e.g., survival by age groups and nodes)
Use advanced plots like swarm plots and strip plots

7. Visualization and Insights

Produce professional-quality charts and graphs
Annotate plots with key findings
Compare survival and non-survival groups visually
Document patterns and anomalies discovered

Key Insights
Based on the exploratory data analysis, here are some key findings:

Axillary Nodes Impact: The number of positive axillary nodes is a strong indicator of survival. Patients with fewer nodes tend to have better survival rates.
Age Distribution: Most patients in the dataset are between 40-60 years old. Age shows a moderate correlation with survival outcomes.
Imbalanced Dataset: The dataset is imbalanced, with more patients surviving 5+ years than those who died within 5 years.
Operation Year: The year of operation shows minimal correlation with survival status, suggesting that medical procedures were relatively consistent during the study period.
Outliers: Some patients have an unusually high number of axillary nodes (50+), which are rare cases that significantly impact survival predictions.
Feature Overlap: There is considerable overlap in feature distributions between survival and non-survival groups, indicating the complexity of survival prediction.

How to Run the Notebook
Prerequisites
Ensure you have the following installed on your system:

Python 3.7 or higher
Jupyter Notebook or JupyterLab

Installation Steps

Clone or download this repository to your local machine
Install required dependencies using pip:

bashpip install pandas numpy matplotlib seaborn jupyter
Or install from a requirements file (if provided):
bashpip install -r requirements.txt

Navigate to the project directory:

bashcd Haberman_EDA

Launch Jupyter Notebook:

bashjupyter notebook

Open the notebook file (Haberman_EDA.ipynb) in your browser
Run all cells sequentially by selecting Cell > Run All or execute cells individually using Shift + Enter

Dataset Placement
Ensure the haberman.csv dataset file is placed in the same directory as the notebook, or update the file path in the data loading section accordingly.
Conclusion
This exploratory data analysis provides valuable insights into the factors affecting breast cancer survival rates in the Haberman dataset. The analysis reveals that the number of positive axillary nodes is the most critical factor influencing patient survival, while age plays a secondary role. The operation year shows minimal impact on survival outcomes.
The visualizations and statistical summaries help understand the dataset's characteristics, identify patterns, and prepare the groundwork for potential predictive modeling. The findings suggest that early detection and treatment (minimizing axillary node involvement) are crucial for improving survival rates.
This EDA serves as a foundation for further research, including machine learning classification models to predict survival status based on patient features.
Future Work
Potential extensions of this project include:

Predictive Modeling: Build classification models (Logistic Regression, Decision Trees, Random Forest, SVM, etc.) to predict survival status
Feature Engineering: Create new features such as age groups, risk categories based on nodes, etc.
Handling Class Imbalance: Apply techniques like SMOTE, undersampling, or class weights to improve model performance
Cross-Validation: Implement k-fold cross-validation for robust model evaluation
Model Comparison: Compare multiple algorithms and select the best-performing model
Deployment: Create a simple web application to predict survival based on user input

Author Information
Author: Haris Ansari


License
This project is open-source and available under the MIT License.
Acknowledgments

Dataset source: UCI Machine Learning Repository
Inspiration: Various data science and EDA tutorials