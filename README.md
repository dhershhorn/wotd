# wotd

A jotto based game with scoring for number of guesses used as well anagrams discovered.

# Rules

You have 20 guesses to identify a secret 5 letter word.
Each guess you make must be a valid 5 letter word.
Correct letters (but not placement) will be revealed to the user for each guess.
Scoring incentivizes using logic to eliminate letters with words that fail to match at all.

# Scoring Details

A perfect score is 100. If you use all 20 guesses and don't find the word your score is 0.

Otherwise, each guess spends up to 5 points from the total possible 100 as follows:
* Empty set (no matching letters): -0 points
* Incorrect guess with some (but not all) matching letters: -1 point per incorrect letter
* Anagram of correct word (all matching letters, different placement): -1 point
* Correct secret word ends the game and loses no points for the final guess

# Feature Backlog

* Add persistent daily high score
* Add authorization to prevent playing more than once per day by player
* Revise UI to include help info and scoring details/tips