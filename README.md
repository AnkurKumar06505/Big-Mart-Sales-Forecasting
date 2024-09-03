This project focuses on predicting product sales across different retail outlets using advanced machine learning techniques. By leveraging a dataset that includes product and outlet information, the goal is to develop a model that accurately forecasts Item_Outlet_Sales. The project involves detailed data preprocessing, exploratory data analysis, and model training using the XGBoost Regressor.

Data
The dataset comprises 8,523 records with 12 features, capturing various aspects of the products and outlets, such as product identifiers, item weight, visibility, outlet characteristics, and the corresponding sales figures.

Key Steps

Data Cleaning:

Addressed missing values by imputing the mean for Item_Weight.
For Outlet_Size, missing values were filled based on the most common size for each Outlet_Type.

Feature Engineering:

Categorical variables were encoded using Label Encoding to convert them into a numerical format suitable for modeling.
Categories in Item_Fat_Content were consolidated to reduce redundancy and ensure consistency in the data.

Exploratory Data Analysis (EDA):

Conducted visualizations to understand the distribution of numerical features like Item_Weight, Item_Visibility, Item_MRP, and Item_Outlet_Sales.
Analyzed categorical variables such as Outlet_Establishment_Year, Item_Type, and Outlet_Location_Type to identify patterns and relationships in the data.

Modeling:

The dataset was split into training (80%) and testing (20%) sets to evaluate model performance.
An XGBoost Regressor model was trained to predict Item_Outlet_Sales, using the processed features.
Model performance was assessed using the R-squared metric, achieving a score of 0.88 on the training set and 0.51 on the test set, indicating the model's potential and areas for further improvement.
