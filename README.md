# Expense Tracker

A simple Python CLI tool to manage daily expenses. Built to practice working with data structures and functional programming in Python.

## 🛠️ Personal Tweak
This project is based on the FreeCodeCamp (FCC) Scientific Computing with Python curriculum. But I tweak the original code by adding error handling

* **Using try-except**: To validate so that the program doesn't error when the input is not a number.

## 🚀 Features
* **Dynamic Data Storage**: Utilizes a list of dictionaries to manage expense records efficiently.
* **Functional Programming**: By implementing Python's built-in `map()` and `filter()` functions combined with `lambda` expressions for streamlined data processing & filtering.
* **Modular Design**: The codebase is organized into distinct, single-responsibility functions `(Add, Print, Total, Filter)` to ensure high maintainability and readability.
* **Interactive CLI Interface**: Features a robust command-line interface powered by a `while` loop, providing a seamless user experience for real time data entry and retrieval.
* **Data Transformation**: Demonstrates effective use of higher order functions to calculate totals and extract specific categories from the dataset.

## 📂 Project Structure
Inside this repository, you will find:
* `track.py` — The main Python script that runs the expense tracker.
* `README.md` — The documentation you are reading right now.

## 💡 How It Works
```bash
User Input -> Main Loop -> Function Logic -> Expenses List (Data Store) -> UI Output
```
* **Initialize**: The program starts with an empty list called `'expenses'`.
* **Menu Selection**: A `while` loop keeps the program running, presenting a menu for different actions.
* **Adding Data**: When an expense is added, the script creates a key-value pair for both `'amount'` and `'category'`, appending it to the collection.
* **Calculations**: To get the total, the program extracts all `'amount'` values from the dictionaries and sums them up using a `lambda function`.
* **Searching**: The filter feature scans the list and returns only the items where the category matches the user's input.  

## ❗ How To Use
1. **Run the script**: Open your terminal and run `python track.py`
2. **Add expenses**: Choose option `1` and enter the amount and category.
3. **View result**: Choose option `2` to see all data, or `3` to see the total sum.
4. **Filter**: Choose option `4` to find specific expenses (e.g., "Food")

## 💻 Example Output
Here, I added my expense of 50,000 food by entering it in option 1, and proving my total expense with option 3

```bash
Expense Tracker
1. Add an expense
2. List all expenses
3. Show total expenses
4. Filter expenses by category
5. Exit

Enter your choice: 1
Enter amount: 50000
Enter category: Food

Expense Tracker
1. Add an expense
2. List all expenses
3. Show total expenses
4. Filter expenses by category
5. Exit

Enter your choice: 3
Total Expenses: 50000.0
```
Note: Of course there's much more than just adding and proving the expenses, you can try it yourself hehe :)