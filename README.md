# 💰 Loan Data Project: Decision Trees vs Random Forest (Which is Better?)

---

## 📌 Project Overview
This project uses **publicly available LendingClub.com loan data** to build predictive models for whether a borrower **fully repaid their loan**.

LendingClub connects borrowers and investors, where investors seek customers with a **high probability of paying back**. This project focuses on comparing **Decision Trees** and **Random Forests** to determine which performs better for loan repayment prediction.

The dataset spans **2007-2010** and has been cleaned of `NaN` values for simplicity.

Data source: [LendingClub](https://figshare.com/articles/dataset/Lending_Club/22121477?utm_source=chatgpt.com)  
Context: [Lending Club 2016 Scandal](https://en.wikipedia.org/wiki/Lending_Club#2016)

---

## 📂 Dataset Features
- **credit.policy**: 1 if customer meets LendingClub.com underwriting criteria, else 0  
- **purpose**: Loan purpose (`credit_card`, `debt_consolidation`, `educational`, `major_purchase`, `small_business`, `all_other`)  
- **int.rate**: Loan interest rate (as a proportion, e.g., 0.11 for 11%)  
- **installment**: Monthly payment amount  
- **log.annual.inc**: Log of annual income  
- **dti**: Debt-to-income ratio  
- **fico**: FICO credit score  
- **days.with.cr.line**: Credit line duration in days  
- **revol.bal**: Revolving balance  
- **revol.util**: Revolving line utilization rate  
- **inq.last.6mths**: Number of credit inquiries in last 6 months  
- **delinq.2yrs**: Past due incidents in last 2 years  
- **pub.rec**: Public derogatory records  

---

## 🎯 Objectives
- Predict **loan repayment status**.
- Compare **Decision Tree** vs **Random Forest** classifiers.
- Evaluate which algorithm performs better.

---

## 🛠 Tools & Libraries
- **Python 3.8+**
- **Pandas** – Data manipulation
- **NumPy** – Numerical operations
- **Matplotlib & Seaborn** – Visualization
- **Scikit-learn** – Machine learning
- **Jupyter Notebook**

---

## 🔍 Workflow
1. Import data science libraries (pandas, numpy, matplotlib, seaborn)
2. Load and inspect data (info(), head(), describe())
3. Perform Exploratory Data Analysis (EDA)
4. Split dataset into training and test sets
5. Initialize and train:
   - Decision Tree Classifier
   - Random Forest Classifier
6. Evaluate models using accuracy and classification metrics
7. Compare results and draw conclusions

---

## 📈 Key Findings
- Both models performed well, but **Random Forest** showed **superior accuracy** and **robustness**.
- Decision Trees tend to overfit, while Random Forest generalizes better.
- Features like **FICO score** and **interest** rate were most influential in predictions.

---

## 📦 Installation & Usage
```bash
# 1️⃣ Clone the repository
git clone https://github.com/Sammy-mercy.git

# 2️⃣ Navigate into the project directory
cd loan_project

# 3️⃣ Install dependencies
pip install -r requirements.txt

# 4️⃣ Open the Jupyter Notebook
jupyter notebook
```
---

## 📌 Future Improvements
- Implement hyperparameter tuning using GridSearchCV
- Explore other ensemble methods (Gradient Boosting, XGBoost)
- Perform feature engineering and scaling for better performance
- Deploy the best model for real-world application

---

## 📜 License
This project is licensed under the MIT License.
