# EXPENSE TRACKER

This is a simple AI-based expense tracking application built in Python. It helps users manage their daily spending by automatically categorizing expenses, tracking budget usage, providing spending summaries, and predicting the next expense using Machine Learning.

## FEATURES

### AUTOMATIC CATEGORIZATION
Uses Machine Learning with **Multinomial Naive Bayes** to automatically classify expenses into categories such as:

- Food
- Travel
- Entertainment
- Stationary
- Fashion
- Essentials

### SELF-LEARNING SYSTEM
If the AI is not confident about an expense category, the user can provide the correct category.

The new information is added to the training data and the Machine Learning model is retrained.

### BUDGET TRACKING
Users can set a budget and monitor their total spending and remaining balance.

### REAL-TIME BUDGET ALERTS

- Warning when 80% of the budget is used
- Alert when the budget is exceeded
- Shows total amount spent
- Shows remaining budget
- Shows percentage of budget used

### EXPENSE MANAGEMENT

Users can:

- Add new expenses
- View all recorded expenses
- Delete selected expenses
- Store expenses in a CSV file

### MONTHLY SUMMARY
Displays the total expenses recorded during the current month along with the number of expenses.

### DATA VISUALIZATION
Displays category-wise spending using a bar graph with **Matplotlib**.

### SPENDING PREDICTION
Uses **Linear Regression** to estimate the next expense based on previously recorded expense amounts.

### GRAPHICAL USER INTERFACE
Provides a simple and easy-to-use desktop interface built using **Tkinter**.

## MACHINE LEARNING

The project uses two Machine Learning techniques:

### 1. NAIVE BAYES

Multinomial Naive Bayes is used for automatic expense category classification.

Example:

    pizza       → Food
    uber        → Travel
    netflix     → Entertainment
    notebook    → Stationary
    shoes       → Fashion
    shampoo     → Essentials

The expense description is converted into numerical features using **CountVectorizer** before classification.

### 2. LINEAR REGRESSION

Linear Regression is used to estimate the next expense based on the trend of previously recorded expenses.

## TECHNOLOGIES USED

- Python
- Tkinter
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- CSV File Storage

## PREREQUISITES

You need Python installed on your system.

Python 3.6 or higher is recommended.

Install the required libraries:

    pip install pandas matplotlib scikit-learn numpy

Tkinter is normally included with Python on Windows.

## HOW TO RUN THE PROGRAM

Save the Python code in a file named:

    expense_tracker.py

Open Terminal or Command Prompt.

Navigate to the folder where the file is saved.

Run the program:

    python expense_tracker.py

## HOW TO USE

### SET BUDGET

1. Enter your budget in the budget field.
2. Click **Set Budget**.

### ADD EXPENSE

1. Enter the expense description.
2. Enter the amount.
3. Click **Add Expense**.
4. The AI automatically predicts the expense category.
5. The expense is saved in `expenses.csv`.

Example:

    Description: Pizza
    Amount: 250

The AI predicts:

    Category: Food

### VIEW ALL EXPENSES

Click **View All Expenses** to see all recorded expenses in a table.

The table displays:

- Date
- Description
- Category
- Amount

### DELETE EXPENSE

Click **Delete Expense**.

Select the expense you want to remove and click **Delete Selected**.

### SHOW SUMMARY

Click **Show Summary** to view:

- Total expenses
- Category-wise expenses
- Bar graph of spending by category

### BUDGET STATUS

Click **Budget Status** to see:

- Total budget
- Total amount spent
- Remaining amount
- Percentage of budget used

### MONTHLY SUMMARY

Click **Monthly Summary** to see the total spending and number of expenses recorded during the current month.

### PREDICT NEXT EXPENSE

Click **Predict Next Expense** to estimate the next expense using Linear Regression.

At least 3 recorded expenses are required for prediction.

## DATA STORAGE

All expenses are stored in a CSV file named:

    expenses.csv

The file contains:

    Date, Description, Category, Amount

The CSV file is automatically created when the first expense is added.

## BUDGET ALERT SYSTEM

The application continuously checks the budget.

    Below 80%       → Normal
    At 80%          → Warning
    At/above budget → Budget Alert
    Above budget    → Budget Exceeded

## PROJECT STRUCTURE

    AI-Expense-Tracker/
    │
    ├── expense_tracker.py
    ├── expenses.csv
    └── README.md

## IMPORTANT NOTES

- Always run the program as a `.py` file.
- Keep `expenses.csv` in the same folder as the Python script.
- Make sure all required libraries are installed.
- A valid positive budget must be entered before adding expenses.
- A minimum of 3 expenses is required for spending prediction.
- The spending prediction is a basic estimate based on previous expense amounts.

## FUTURE IMPROVEMENTS

- Add a modern and attractive UI design
- Add user login and authentication
- Replace CSV storage with SQLite or MySQL
- Add income and savings tracking
- Add weekly and yearly reports
- Add expense editing functionality
- Improve Machine Learning accuracy
- Add advanced spending prediction
- Add interactive dashboards
- Convert the application into a Windows `.exe`
- Develop a web or mobile version

## SCREENSHOTS

Add your application screenshots below.

Example:

![Expense Tracker Screenshot](screenshot1.png)

![Expense Summary Screenshot](screenshot2.png)

## PROJECT OBJECTIVE

The main objective of this project is to create a simple AI-based expense management system that combines **Python, Machine Learning, data analysis, data visualization, and GUI development** to help users manage and understand their spending.
