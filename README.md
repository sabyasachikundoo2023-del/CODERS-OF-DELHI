🇮🇳 CODERS-OF-DELHI: The Pure-Python Data Science Challenge
📌 Project Overview
Coders-of-Delhi (CoD) is a social network simulation designed to test fundamental data engineering and algorithmic skills. As a Data Scientist Intern, you are tasked with managing the platform's social graph under a strict technical constraint: Zero external libraries. No Pandas, no NumPy, and no Scikit-learn.

This repository documents a 1-month intensive journey from raw data handling to building a personalized recommendation engine using only built-in Python modules.

📂 Repository Structure
The project is divided into four critical phases, each represented by a dedicated module:

File	Phase	Description
01_Introduction.ipynb	Data Ingestion	Initial loading and structured display of the user JSON database.
02_data_cleaning.ipynb	Data Integrity	Handling missing names, deduplicating friend lists, and removing inactive users.
03_people_you_may_know.ipynb	Graph Logic	An algorithm to suggest new connections based on mutual friend counts.
04_pages_you_might_like.ipynb	Recommendation	Interest-based page suggestions using shared liked-page intersections.
🛠️ Key Features
1. Intelligent Data Cleaning
Automated pipeline to ensure the "Delhi Coder Graph" stays healthy by:

Stripping whitespace and removing users with missing names.

Standardizing friend lists using set() logic to prevent duplicate connections.

Removing "Ghost Users" who have neither friends nor liked pages.

2. "People You May Know" (PYMK) Engine
A custom graph traversal algorithm that:

Identifies non-friends with mutual connections.

Ranks suggestions based on the density of mutual friends.

3. Collaborative Interest Discovery
Suggests new community pages to users by:

Analyzing common interests between the target user and others.

Calculating a "Shared Interest Score" to prioritize high-value page recommendations.

🚀 Getting Started
Technical Requirements
Python 3.12+

Standard Modules: json, collections, math

Running the Simulation
To view the current state of the Delhi network and see the recommendation engine in action:

Bash
# Example execution of the recommendation logic
python 03_people_you_may_know.ipynb
📈 Progress Tracking
[x] Task 1: Load and parse raw JSON dumps.

[x] Task 2: Implement data cleaning and deduplication logic.

[x] Task 3: Build a "Mutual Friend" suggestion engine.

[x] Task 4: Develop interest-based page recommendation scoring.

👨‍💻 About the Author
Developed by a 1st year  CSE student focused on mastering Data Science and Machine Learning from the ground up. This project serves as a foundation for building scalable algorithms without the "crutch" of heavy frameworks.
