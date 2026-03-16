Project Overview

This project aims to predict the price of Airbnb listings using machine learning techniques based on listing characteristics such as location, amenities, host information, and property attributes.
The objective is to build a predictive model capable of estimating the logarithm of the listing price (log_price) using structured and unstructured data from Airbnb listings.

This project demonstrates the full Data Science workflow, including:
- Exploratory Data Analysis (EDA)
- Data cleaning and preprocessing
- Feature engineering
- Machine learning model training
- Model evaluation and comparison
- Prediction generation for unseen data

Dataset
The dataset contains information about Airbnb listings, where each row represents a listing and its associated attributes.

Target Variable
log_price: Logarithm of the listing nightly price (target variable used for prediction)

Example Features
| Feature                 | Description                               |
| ----------------------- | ----------------------------------------- |
| `property_type`         | Type of property (Apartment, House, etc.) |
| `room_type`             | Entire home, private room, shared room    |
| `accommodates`          | Number of people the listing accommodates |
| `bathrooms`             | Number of bathrooms                       |
| `bedrooms`              | Number of bedrooms                        |
| `beds`                  | Number of beds                            |
| `amenities`             | List of amenities available               |
| `city`                  | City where the listing is located         |
| `latitude`, `longitude` | Geographical coordinates                  |
| `number_of_reviews`     | Number of reviews                         |
| `review_scores_rating`  | Overall rating score                      |
| `host_response_rate`    | Host responsiveness percentage            |

Project Workflow

1️⃣ Exploratory Data Analysis (EDA) : 
The first step consisted of exploring the dataset to better understand its structure and characteristics:
- Distribution of numerical variables
- Missing values analysis
- Correlation analysis
- Outlier detection
- Data visualization (histograms, heatmaps, etc.)
These insights guided the preprocessing and feature engineering steps.

2️⃣ Data Preprocessing : 
Several preprocessing techniques were applied:
- Handling missing values
- Encoding categorical variables
- Feature normalization / scaling
- Cleaning textual features
- Date feature transformation
- Feature selection

3️⃣ Feature Engineering : 
New variables were created to improve model performance, such as:
- Host experience (based on host_since)
- Review activity indicators
- Processed amenities features
- Location-related insights
  
4️⃣ Machine Learning Models :
Several supervised learning models were tested and compared:
- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Models
The models were evaluated using appropriate regression metrics.

5️⃣ Model Evaluation : 
Model performance was assessed using:
- RMSE (Root Mean Squared Error)
- Train/Test split validation
- Cross-validation for robustness
The best-performing model was then used to generate predictions for the test dataset.

Project Structure
Airbnb-Price-Prediction/
│

├── project.ipynb              # Main notebook (EDA + modeling)

├── airbnb_train.csv           # Training dataset

├── airbnb_test.csv            # Test dataset

├── prediction.csv             # Final predictions

├── prediction_example.csv     # Submission format example

└── README.md                  # Project documentation

Technologies Used
- Python
- Pandas
- NumPy
- Scikit-Learn
- Matplotlib
- Seaborn
- Jupyter Notebook

Key Skills Demonstrated
- Data exploration and visualization
- Data preprocessing and cleaning
- Feature engineering
- Supervised machine learning
- Model evaluation
- Reproducible data science workflow

Possible Improvements
- Future improvements could include:
- Natural Language Processing on the description field
- Advanced feature engineering on amenities
- Hyperparameter optimization
- Use of advanced models such as XGBoost, LightGBM, or CatBoost
- Geospatial analysis based on latitude and longitude
