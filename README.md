# Bangalore Property Insights & Value Predict 
This project aims to predict property prices in Bangalore by scraping data from the Makkan website, cleaning and extracting features from the data, and building machine learning models. The process is implemented using Python and various libraries, organized into separate Jupyter Notebook files for each major step.

## Table of Contents

1. Project Overview
2. Data Collection
3. Data Cleaning
4. Feature Extraction
5. Model Building
6. Results
7. Tools & Libraries
8. How to Run
9. Future Enhancements
10. Contributing
11. Analysis Dashboard

## Project Overview

This project aims to predict property prices in Bangalore using machine learning models trained on data collected from the Makkan website. The project workflow involves four primary stages: data scraping, data cleaning, feature extraction, and model building. By dividing the tasks into separate steps, the project ensures a systematic approach to transforming raw web data into a highly accurate predictive model capable of estimating property prices.

## Data Collection (Data_scraping.ipynb)

### Objective:
Collect raw data on Bangalore properties directly from the Makaan website (https://www.makaan.com/) using web scraping techniques tailored for dynamic content.
### Methodology:

**Tool:** Utilize `Selenium` for dynamic content handling.

**Data Points:**  Extract details like bedrooms, bathrooms, location, price, and size.

### Challenges Faced:

**Dynamic Content Handling:**  Handled with Selenium for scrolling, clicking, and loading hidden data.

**Data Integrity:**  Validated data against listings and handled timeouts/delays.

**Output:**  Comprehensive CSV dataset containing scraped features.

## Data Cleaning (cleaning.ipynb)

### Objective: 

Refine the scraped data by addressing inconsistencies like missing values and duplicate entries.
### Steps:
**Missing Values:** Handle missing values with imputation or removal strategies. Duplicate removal and data type normalization are also performed.

**Outlier Detection:** Identify and handle outliers in numeric fields using z-score analysis.

**Output:** Cleaned CSV dataset ready for further processing.

## Feature Extraction (featureextraction.ipynb)

### Objective:
Extract additional features and categorize existing data.

### Steps:

**No. of Bathrooms Extraction:** Develop a function to extract the number of bathrooms from the description.

**No. of BHK:** Develop a function to extract the number of BHK from the Property column

**Locality Standardization:** Clean locality names for consistent entries.

**Output:** Enriched dataset with extracted features (e.g., number of bathrooms) saved as ML_ready.csv.

## Model Building (ML_models.ipynb)

### Objective:
Develop and evaluate machine learning models for price prediction.
### Models: 
 * `Linear Regression`
   
 * `Decision Tree`
     
 * `Random Forest`
 
### Approach:
Data split (training/testing) for model evaluation and `k-fold cross-validation` for stability assessment.

Hyperparameter tuning to optimize model performance.

Evaluation using `Mean Absolute Error (MAE)` , `Mean Squared Error (MSE)` , and `R-squared.`

**Output:** The best-performing model saved for potential deployment.
## Tools & Libraries

**`Python:`** Core language for development.

**`Selenium:`** Web scraping for dynamic content. (Replaced Beautiful Soup)

**`Pandas & NumPy:`** Data manipulation and analysis.

**`Scikit-learn:`** Machine learning algorithms and evaluation metrics.

**`Matplotlib & Seaborn:`** Data visualization.

**`VS Code (Jupyter Extension):`** Interactive development environment.



## How to Run

**Clone the repository.**

  Install required libraries  `(pip install -r requirements.txt)`.

**Execute Jupyter Notebooks:**

* Data_scraping.ipynb 

* cleaning.ipynb 
 
* featureextraction.ipynb 

* ML_models.ipynb 

## Future Enhancements

Introduce advanced feature engineering (e.g., proximity to amenities).

Experiment with advanced machine learning models.

Develop a deployment solution (web application or API).
## Contributing
We welcome contributions to enhance this project. If you have suggestions or improvements, please fork the repository, create a new branch with your changes, and submit
We welcome contributions! Fork the repository, create a branch with your changes, and submit a pull request.


## Analysis Dashboard
![Screenshot 2024-09-20 221507](https://github.com/user-attachments/assets/e120c2a1-1417-4718-be20-4ca2046505e8)
