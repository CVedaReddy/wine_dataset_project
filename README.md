![image](https://github.com/user-attachments/assets/e991bcc3-5626-4864-a87f-7a68fd688102)# wine_dataset_project

This dataset contains various physicochemical properties and quality ratings for red wine samples. The features (fixed acidity, volatile acidity, citric acid, etc.) are used to predict the quality of the wine, which is rated on a scale from 0 to 10. Each column represents a different aspect of the wine's composition or its assessed quality.

Wine Quality - Red Wine Dataset Description

1.	Fixed Acidity (fixed acidity)
o	Description: Fixed acids are non-volatile acids that do not evaporate easily.
o	Units: grams per liter (g/L)

3.	Volatile Acidity (volatile acidity)
o	Description: Volatile acids can evaporate and contribute to the wine's aroma and taste.
o	Units: grams per liter (g/L)

4.	Citric Acid (citric acid)
o	Description: Citric acid is a weak organic acid that adds freshness and flavor to the wine.
o	Units: grams per liter (g/L)

5.	Residual Sugar (residual sugar)
o	Description: Residual sugar is the amount of sugar remaining after fermentation stops.
o	Units: grams per liter (g/L)

7.	Chlorides (chlorides)
o	Description: Chlorides represent the amount of salt in the wine.
o	Units: grams per liter (g/L)

9.	Free Sulfur Dioxide (free sulfur dioxide)
o	Description: Free sulfur dioxide is the amount of SO2 that is not bound and is available to act as an antimicrobial and antioxidant.
o	Units: milligrams per liter (mg/L)

11.	Total Sulfur Dioxide (total sulfur dioxide)
o	Description: Total sulfur dioxide includes both bound and free forms of SO2.
o	Units: milligrams per liter (mg/L)

13.	Density (density)
o	Description: Density is the mass per unit volume of the wine, influenced by the amount of sugar and alcohol.
o	Units: grams per cubic centimeter (g/cm³)

15.	pH (pH)
o	Description: pH measures the acidity or alkalinity of the wine. Lower pH values indicate higher acidity.
o	Units: pH scale (dimensionless)

17.	Sulphates (sulphates)
o	Description: Sulphates are added to wine to prevent spoilage and oxidation.
o	Units: grams per liter (g/L)

19.	Alcohol (alcohol)
o	Description: The alcohol content of the wine.
o	Units: percentage by volume (% vol)

21.	Quality (quality)
o	Description: The quality score of the wine, typically based on sensory data (taste, aroma, etc.).
o	Units: score (integer scale from 0 to 10)


Concepts used: 

Data Preprocessing – 
This process mainly involves cleaning and transforming raw data into a format that models can understand and learn from effectively.

Data Cleaning involves: 
Handle Missing Values:
Removing rows or columns and filling them with mean, median, or mode
Remove Duplicates:
Drop identical rows
Fix Errors or Outliers

Data Transformation involves:

Normalisation or Scaling: This involves bringing all numerical features to the same scale using - 
Min-Max Scaling
Standardisation (Z-score)
Encoding Categorical Data: Process of converting non-numeric values to numbers - 
One-Hot Encoding

Feature Selection
This step involves selecting important features and creating new features from existing ones

Data Splitting
Divide the dataset into:
Training set
Testing set

2. Correlation – 
 
Correlation measures the relationship between two variables, how one variable changes in response to another.

For strength: 0–0.3: Weak, 0.3–0.7: Moderate, 0.7–1.0: Strong 
For direction: Positive values = As one metric increases, the other tends to increase, Negative values = As one metric increases, the other tends to decrease. 
0 means no correlation, +1 means perfect positive correlation, -1 means perfect negative correlation 

3. Finding maximum, minimum and average

In data analysis, maximum and minimum helps us to identify the range of values in a dataset. . min() function returns the smallest value in dataset. .max() function returns the largest value in the dataset. 
Accuracy score is a used to evaluate how a classification model performs. It is equal to ratio of Number of Correct Predictions / Total Number of Predictions

4. Decision Tree Classifier- 

It is a supervised machine learning algorithm used for both classification and regression tasks. It works by splitting the data   into subsets based on the value of input features, forming a tree-like structure.

How this works: 
Root Node: Start with the entire dataset.
Splitting: to find the best feature and value to split the data using a following criteria :
Gini Index (default for classification)
Entropy (for Information Gain)
Internal Nodes: Represent decisions based on feature values.
Leaf Nodes: Represent final output either class label or value .
Continue splitting until a stopping criterion is met (i.e.,  max depth or pure leaf).

5. Random Forest Classifier- 
  
It is an ensemble machine learning algorithm used for classification and regression tasks. It builds multiple decision trees and combines their outputs for better accuracy and robustness.
Random Forest is made of many decision trees trained on random subsets of the data.
Random Feature Selection: At each split, a random subset of features is considered 

Hyperparameters used are :
n_estimators: Number of trees in the forest.
max_features: Max number of features considered at each split.
max_depth: Max depth of each tree.
criterion: Function to measure the quality of a split (gini or entropy).


