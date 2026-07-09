
E-Commerce Purchase Intention Model

📌 Overview
This project builds a machine learning classification model that analyzes consumer behavior data from web analytics (such as click-stream data, page types, and session duration) to predict whether a customer will make a purchase during their visit. By predicting purchase intention in real-time, e-commerce platforms can serve targeted promotions to customers who are on the fence.

 🗂️ What is Included in this Repository
`online_shoppers_intention.csv`**: The raw dataset containing 12,330 web sessions. It includes features like page views (Administrative, Informational, Product Related), session duration, browser type, operating system, and the target variable (`Revenue`).
-`final_code.py`: The complete, end-to-end Python script. This file:
  - Performs data cleaning and feature engineering (e.g., converting Boolean variables, applying Ordinal Encoding).
  - Builds a robust Machine Learning Pipeline using `scikit-learn`.
  - Handles class imbalance automatically using **SMOTE**.
  - Selects the optimal features using **SelectKBest**.
  - Trains and evaluates the best performing model (**MLPClassifier**).

 🚀 How to Run the Project Locally

Follow these steps to run the machine learning pipeline on your own machine.

 Step 1: Clone the Repository
Open your terminal or command prompt and download the code:
cmd
git clone [https://github.com/Rajesh-2285/Datascience-projects.git](https://github.com/Rajesh-2285/Datascience-projects.git)
cd Datascience-projects/purchase_intention_model

------------------------------------------------------------------------------------

Step 2: Install Required Libraries
This project relies on several standard data science and machine learning libraries. Install them by running:
pip install pandas numpy scikit-learn imbalanced-learn matplotlib seaborn xgboost lightgbm
------------------------------------------------------------------------------------

Step 3: Run the Script
Ensure you are in the same folder as the online_shoppers_intention.csv file, and execute the Python script:

python final_code.py

------------------------------------------------------------------------------------

📊 Expected Output & Results
When you run the script, it will print out its step-by-step progress in the terminal. After training the pipeline, it will output the final evaluation metrics.

The MLPClassifier (Multilayer Perceptron) achieves the following performance:

Overall Accuracy: ~88%

ROC/AUC Score: ~0.83 (Test Data) / 0.90 (Training Data)

True Negative Rate: Correctly predicts 90% of customers who will not purchase.

True Positive Rate: Correctly identifies 77% of customers who will purchase.

-----------------------------------------------------------------------------------------
One Last Tip:
Before you commit this `README.md` to GitHub, ensure that `final_code.py` and `online_shoppers_intention.csv` are actually in the root folder of that specific repository, or update the path in the `README.md` if they are tucked inside a subfolder! 

You are now fully prepared to present these projects to recruiters. You have the code, the documentation, and the cloud-deployed API. **Go get those interviews!
