# Usage
1. Prepare the Dataset: Make sure you have a CSV file (skaters.csv) containing the player statistics with the following columns:
  - name: The name of the player.
  - season: The season of the statistics (e.g., 2023).
  - gameScore: The total game score for the player.
  - games_played: The number of games played by the player.
2. Run the Script: Modify the file_path variable in the script to point to your CSV file. Then run the script:
  - python player_rating_model.py
3. Input Player Names: The script will prompt you to enter the player's name for whom you want to calculate the rating. You can type "exit" to stop the program.

# Functionality
  - GS/GP Calculation: The model calculates the Game Score per Game (GS/GP) for each player.
  - Regularization: If a player has played fewer than 50 games, the model applies a regularization technique by averaging their score with the mean GS/GP of players who have played fewer games.
  - Rating Output: The script outputs the calculated rating for the specified player and season.

# Data Requirements
The dataset used must be in CSV format and include the following columns:
  - name (str): The player's name.
  - season (int): The season (e.g., 2023).
  - gameScore (float): The player's total game score.
  - games_played (int): The number of games the player has played.

The data used is from MoneyPuck.com!
