Baseball Data Analysis with NumPy
Overview
This project uses NumPy to analyze a baseball statistics dataset loaded from a CSV file. It demonstrates how to:

Load CSV data into a NumPy array while skipping the header row

Inspect the shape and sample rows of the dataset

Filter players based on conditions (e.g., home runs > 20)

Calculate averages and counts on filtered data

Use logical operations like np.any() and np.all() to answer yes/no questions about the dataset

Combine multiple filters with logical AND to refine queries

Dataset Description
The dataset (baseball.csv) contains numerical stats for 50 players, each with 6 attributes per row, such as height, batting average, home runs, etc. 
The header row is skipped when loading.

Key Functionalities
Load the CSV data (excluding the header) with np.genfromtxt.

Display the dataset shape and the first two players’ stats.

Filter and display players who hit more than 20 home runs.

Calculate the average number of home runs and count players who meet that threshold.

Check if any player hit more than 50 home runs using np.any().

Check if all players are taller than 150 cm using np.all().

Filter players who hit more than 20 home runs and have a batting average above 0.250, then display them.

How to Run
Ensure Python 3 and NumPy are installed:
pip install numpy
Place baseball.csv in the same directory as the script.

Run the script with:
python baseball_analysis.py
Sample Output Insights
The data shape prints as (50, 6) indicating 50 players with 6 stats each.

First two players’ stats are displayed.

Players with more than 20 home runs are listed, along with their average home runs (approx. 24.5) and count (19 players).

The script confirms no player has more than 50 home runs.

All players are taller than 150 cm.

The final filtered list shows players meeting both the home run and batting average criteria.

Notes
This example illustrates basic data filtering and summary statistics with NumPy arrays. It’s a useful pattern for exploratory data analysis 
on numeric datasets without needing pandas or other libraries.
