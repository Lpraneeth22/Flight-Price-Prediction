🛫 Flight Price Prediction 
📘 Overview

The Flight Price Prediction Pipeline is a data science project designed to analyze airline fare data and build predictive models to estimate flight ticket prices.
The project demonstrates the end-to-end data science workflow — from data extraction to EDA, feature engineering, model training, and evaluation.

🧩 Table of Contents

Introduction

Dataset Overview

Data Validation & Cleaning

Exploratory Data Analysis (EDA)

Modeling

Results

Installation

Usage

Technologies Used

Author

🔍 Introduction

Air travel pricing is dynamic and influenced by various factors such as airline, source, destination, total stops, and duration.
This project aims to explore flight fare data, uncover key insights, and build a machine learning model capable of predicting flight ticket prices accurately.

📊 Dataset Overview

Source: MySQL Database (table: data_train_clean)

Columns include:

Airline

Date_of_Journey

Source & Destination

Total_Stops

Duration

Price

🧹 Data Validation & Cleaning

Handled inappropriate data types

Added missing columns where necessary

Checked for missing/null values

Standardized categorical and numerical fields

📈 Exploratory Data Analysis (EDA)

EDA was performed using Matplotlib, Seaborn, and Plotly to visualize:

Flight price distribution

Airline-wise average fares

Relationship between stops, duration, and price

🤖 Modeling

Steps include:

Feature Selection & Encoding – One-Hot Encoding for categorical columns.

Train-Test Split – Dividing dataset into training and test sets.

Model Training – Various regression models were tested (e.g., Random Forest, XGBoost).

Hyperparameter Tuning – To optimize performance using GridSearchCV.

📈 Results

Achieved a good prediction accuracy for flight fares.

Insights show airline and total stops as the most influential factors.

⚙️ Installation

To set up this project locally:

# Clone the repository
git clone https://github.com/yourusername/Fightprice_pipeline.git
cd Fightprice_pipeline

# Install dependencies
pip install -r requirements.txt


Dependencies include:

pandas
numpy
matplotlib
seaborn
plotly
sqlalchemy
pymysql
scikit-learn

🚀 Usage

Ensure your MySQL database is running and configured in the notebook:

data = create_engine("mysql+pymysql://root:yourpassword@localhost/Airline")


Run the notebook:

jupyter notebook Fightprice_pipeline.ipynb


Execute cells step-by-step to load data, visualize trends, and train models.

🧠 Technologies Used

Python

MySQL

Pandas, NumPy

Matplotlib, Seaborn, Plotly

Scikit-learn

SQLAlchemy

👨‍💻 Author

L. Praneeth
📚 B.Tech in Mechanical Engineering | Aspiring Data Scientist
💼 Focus: Data Analysis, Machine Learning, and AI
