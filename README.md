# Payment Delay Prediction
📌 Project Overview
HighRadius is a B2B company where clients are expected to make payments by a specified due date for their orders. However, in many cases, these payments are delayed. The objective of this project is to predict the actual payment delay using historical payment data. This prediction can help the company proactively manage cash flow and follow-ups with clients.

🎯 Problem Statement
Goal: Predict the number of days by which a client will delay the payment, based on historical invoice and payment behavior.
We framed this as a classification problem, where the delay is categorized into bins (e.g., on-time, short delay, long delay). A Random Forest Classifier is used for the prediction task.

🔍 Steps Involved
1. 📊 Exploratory Data Analysis (EDA)
        Analyzed missing values, data types, and class distribution.
        Explored key features like due_date, clear_date, invoice_date, baseline_create_date, and total_open_amount.
        Handled outliers and inconsistencies in the payment and invoice dates.

2. 📈 Data Visualization
        Created histograms and bar plots to observe the distribution of delays.
        Correlation matrix to understand relationships between features.
        Time-series plots showing monthly trends in delays.

3. 🧬 Feature Engineering & Analysis
        Derived features like delay_days = clear_date - due_date.
        Converted dates to numerical features like day, month, and year.
        One-hot encoded categorical features such as customer names or IDs.
        Analyzed feature importance using tree-based models and correlation metrics.

4. 🤖 Predictive Modeling
        Defined delay categories (e.g., on-time, 1-15 days late, 16-30 days late, etc.).
        Split data into training and test sets.
        Used Random Forest Classifier for prediction due to its robustness and feature importance interpretation.
        Evaluated model using metrics such as accuracy, precision, recall, F1-score, and confusion matrix.

5. 📉 Model Evaluation & Interpretation
        Performed hyperparameter tuning using GridSearchCV.
        Plotted feature importance to understand key drivers of payment delay.
        Visualized confusion matrix and classification report to assess performance.

🛠️ Tech Stack
        Language: Python
        Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn
        Model: Random Forest Classifier
        Environment: Jupyter Notebook / Google Colab
