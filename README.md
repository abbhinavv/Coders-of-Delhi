# Coders-of-Delhi
A pure Python project that cleans and structures messy user data, then builds a “People You May Know” feature by analyzing mutual friends—similar to friend recommendations on social networks.

👥 CodeBook User Analysis & Friend Recommendation System
📖 Project Overview

This project simulates a real-world data analytics task assigned by a manager at CodeBook. The goal is to:

Load and explore a messy user data dump

Clean and structure the data using pure Python

Build a "People You May Know" feature based on mutual connections

The project demonstrates essential data preprocessing skills and basic social network analysis without relying on external libraries like Pandas or NetworkX.

🎯 Objectives
✅ Data Cleaning & Structuring

Handle missing values

Remove duplicate and inconsistent records

Standardize data formats (IDs, names, connections, etc.)

🤝 Friend Recommendation System

Analyze user connections

Identify mutual friends

Suggest new connections based on shared relationships

🛠️ Technologies Used

Python (Pure Python)

Built-in modules only (collections, itertools, etc.)

📂 Project Structure
codebook-user-analysis/
│
├── data/
│   └── users_data.txt / users_data.json
│
├── data_cleaning.py
│   ├── load_data()
│   ├── clean_missing_values()
│   ├── remove_duplicates()
│   └── standardize_data()
│
├── recommendations.py
│   ├── find_mutual_friends()
│   └── people_you_may_know()
│
├── main.py
│   └── Runs full pipeline
│
└── README.md

🔍 Data Cleaning Steps

Missing Values Handling

Removed users with invalid IDs

Filled missing friend lists with empty lists

Duplicate Removal

Eliminated duplicate user records

Ensured unique user IDs

Data Standardization

Converted friend lists to consistent formats

Normalized user identifiers

🤖 “People You May Know” Logic

A user is recommended another user if:

They are not already connected

They share one or more mutual friends

Example:
User A → Friends: [B, C]
User D → Friends: [B, C]

Recommendation:
A ↔ D (2 mutual friends)

▶️ How to Run
python main.py

📌 Sample Output
People You May Know for User 101:
- User 205 (3 mutual friends)
- User 319 (2 mutual friends)

🚀 Future Improvements

Rank recommendations by number of mutual friends

Add weighted relationships

Convert to Pandas-based pipeline

Build a REST API or UI layer

🧠 Key Learnings

Real-world data is messy and needs preprocessing

Graph-like problems can be solved using basic Python

Mutual friend logic is foundational for social platforms

👨‍💻 Author

Built as a hands-on data analytics and algorithmic thinking project.
