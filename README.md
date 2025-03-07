# Hybrid_RAG_FineTuned_LLM_using_NFL Draft Player 

This repository contains a Python script that scrapes NFL Draft player data from NFL Draft Buzz, processes the data, and enables retrieval of player insights using a language model.

Features

Scrapes player details, including name, position, team, strengths, weaknesses, and scouting report summary.

Saves data into a structured CSV file.

Uses FAISS for efficient similarity search based on player scouting reports.

Implements a language model (GPT-2) to generate insights based on player attributes.

Requirements

To run this script, install the required dependencies:

pip install requests beautifulsoup4 pandas faiss-cpu torch transformers sentence-transformers datasets

Usage

Run the script using:

python nfl_draft_scraper.py

Data Processing

The script scrapes player data from multiple pages.

The collected data is saved as nfl_players_data.csv.

The data is processed to extract structured player information.

Retrieval & AI Model

FAISS index is built for similarity search.

The model can generate answers based on player scouting reports.

Example query:

query = "Tell me about players with strong upper body strength."
answer = generate_answer(query)
print("Q:", query)
print("A:", answer)

Output

The output includes:

CSV file with player scouting data.

AI-generated insights based on scouting reports.
