# Coders-of-Delhi
A pure Python project that cleans and structures messy user data, then builds a “People You May Know” feature by analyzing mutual friends—similar to friend recommendations on social networks.

# 👥 CodeBook User Analysis & People You May Know System

## 📖 Project Overview

This project simulates a real-world task assigned at **CodeBook**, where the objective is to analyze a messy user data dump using **pure Python**, clean and structure the data, and finally build a **“People You May Know”** recommendation feature based on mutual friends.

The project focuses on data preprocessing, logical problem-solving, and basic social network analysis without using external libraries like Pandas or NetworkX.

---

## 🎯 Objectives

### 1. Data Loading & Exploration
- Load raw user data
- Understand structure and inconsistencies

### 2. Data Cleaning & Structuring
- Handle missing values
- Remove duplicate or inconsistent records
- Standardize data formats

### 3. Friend Recommendation System
- Analyze mutual friends
- Recommend new connections
- Avoid suggesting existing friends

---

## 🛠️ Technologies Used

- Python (Pure Python)
- Built-in modules only

---

## 📂 Project Structure


codebook-user-analysis/
│
├── data/
│ └── users_data.txt
│
├── data_cleaning.py
│ ├── load_data()
│ ├── handle_missing_values()
│ ├── remove_duplicates()
│ └── standardize_data()
│
├── recommendations.py
│ ├── find_mutual_friends()
│ └── people_you_may_know()
│
├── main.py
│ └── Execute full workflow
│
└── README.md


---

## 🧹 Data Cleaning Process

- Removed users with missing or invalid IDs  
- Filled missing friend lists with empty lists  
- Eliminated duplicate user entries  
- Standardized user and friend ID formats  

---

## 🤝 People You May Know Logic

A user is recommended another user if:
- They are **not already friends**
- They share **one or more mutual friends**

### Example

User A → Friends: [B, C]
User D → Friends: [B, C]

Recommendation:
A ↔ D (2 mutual friends)


---

## ▶️ How to Run

```bash
python main.py

People You May Know for User 101:
- User 205 (3 mutual friends)
- User 319 (2 mutual friends)

🚀 Future Enhancements

Rank recommendations by mutual friend count

Improve performance for large datasets

Add Pandas-based implementation

Build an API or frontend interface

🧠 Key Learnings

Handling messy real-world data

Data cleaning using core Python

Implementing social network recommendation logic

Working with graph-like relationships

👨‍💻 Author

Created as a Python data analysis and algorithmic practice project.

