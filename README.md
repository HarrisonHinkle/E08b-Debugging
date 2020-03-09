# E08b-Debugging

This was an exercise in my Game Technolgy Course at IU where we practiced debugging. We were given a Godot file with a simple 2D platformer inside and our goal was to find an fix 8 bugs placed in there by our instructor. 

In the end, these were the 8 fixes I made:

1.	Changed line 24 of PlayerData.gd from deaths = new_scores to deaths = new_value so it wouldn’t say a variable is undeclared 
2.	Fixed indentation on lines 22 and 23 of Portal2D
3.	Changed sytanx error on UserInterface.gd by changing line 37 from score_label.Text = “Score: %s" % PlayerData.score to score_label.text = "Score: %s" % PlayerData.score
4.	Deleted line 20 on PlayerData.gd because it was locking the players score to 5 
5.	Toggled visibility on the enemy sprite so it could be seen in game
6.	Deleted line 17 on enemy.gd as it made enemies float into the sky
7.	Changed line 8 of EndScreen.gd from result.text = result.text % [PlayerData.Score, PlayerData.deaths] to result.text = result.text % [PlayerData.score, PlayerData.deaths] so it wouldn’t result in an error
8.	Changed line 53 of Player.gd from PlayerData.deaths += 10 to PlayerData.deaths += 1 so it wouldn’t count each player death as ten player deaths
