# Overview of the Leaderboard
The leaderboard is where scores of players are displayed. Currently the scores of the player are not being stored within the leaderboard.
What is being implemented is a function to grab the score from the player after losing/winning a game and storing it into a textfile. 

# Pseudocode for this feature

**In WinPane / LosePane**

``` `function` storePlayerScore()

	score <= player.getScore()

	application.sendScore(score)

```

**In MainApplication**

``` `function` sendScore(score)

	leaderboard.store(score)

```

**In LeaderBoard**

``` `function` store(score)

	while( leaderboard end of file not reached)

		check score > score from file

			temp <= score from file

			score from file <= score

			score <= temp

	

```

