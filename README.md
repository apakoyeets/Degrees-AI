# Degrees-AI
# Degrees of Separation

This project determines the shortest path (degrees of separation) between two actors based on the movies they've starred in. Inspired by the "Six Degrees of Kevin Bacon" concept, it uses breadth-first search (BFS) to find the shortest connection through shared films.

## What It Does

Given any two actor names, the program outputs the shortest sequence of co-starring roles connecting them.

### Example:

## How It Works

- Loads movie and actor data from `.csv` files (based on IMDb data).
- Models the problem as a graph where:
  - Nodes = actors
  - Edges = movies shared with another actor
- Uses Breadth-First Search (BFS) to find the shortest path from the source actor to the target actor.

## Files

- `degrees.py` — Main program logic.
- `util.py` — Includes Node and QueueFrontier classes to support BFS.
- `large/` and `small/` — Contain IMDb-like datasets in CSV format:
  - `people.csv`: actor IDs and names
  - `movies.csv`: movie IDs and titles
  - `stars.csv`: connections between actors and movies

## How to Run

1. Make sure you have Python 3.12 or later installed.
2. Download the dataset and script files.
3. Run the program:
4. Enter two actor names when prompted.

## AI Concepts Involved

- **Graph Search**: Models relationships as a graph and uses BFS to explore.
- **Search Algorithms**: Implements uninformed search to guarantee the shortest path.
- **Disambiguation Handling**: If multiple actors have the same name, the user is prompted to choose the correct one based on ID and birth year.

## Why It Matters

This project demonstrates how AI concepts like graph traversal and pathfinding can solve real-world problems involving networks and relationships — such as finding social or professional connections between people.

---

Created for CS50’s Introduction to Artificial Intelligence with Python.
