# Scoregame-dict.py

This code implements a word scoring game where players earn points based on the letters in the words they play. It consists of several components:

1.Letter-to-Points Mapping: The game assigns point values to each letter of the alphabet. The letters are stored in a list called letters, and their corresponding point values are stored in a list called points. These two lists are used to create a dictionary called letter_to_points, where each letter is mapped to its respective point value.

2.Scoring Words: The code defines a function called score_word that takes a word as input and calculates its point value. It initializes a variable point_total to 0 and iterates through each letter in the word. For each letter, it retrieves its point value from the letter_to_points dictionary using the get() method. If the letter is not found in the dictionary, it defaults to 0. The point values of all letters in the word are summed up and returned as the total point value of the word.

3.Player Scores: The code introduces a dictionary called player_to_words, which maps each player to a list of words they have played. It then creates an empty dictionary called player_to_points to store the total points earned by each player.

-The code iterates through the items in player_to_words using a for loop, with each player and their list of words assigned to the variables player and words respectively.

-For each player, a variable player_points is initialized to 0.

-Another loop is used to iterate through each word in the player's list of words.

-For each word, the score_word function is called to calculate its point value, which is then added to the player_points.

-Finally, the total player_points is assigned to the respective player in the player_to_points dictionary.

4.Printing Player Scores: The code prints the player_to_points dictionary, which represents the current standings of the game. Each player is displayed along with their corresponding total points.

The code provides a simple example of how to score words in a game and track the scores of multiple players.
