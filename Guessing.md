```mermaid
graph TD;
    A([Start])-->B[Game Master rolls a 6 sided die];
    B-->C[/Player guesses a number between 1 and 6/];
    C-- if numberRolled = numberGuessed -->D[Player Wins];
    C-- if numberRolled != numberGuessed -->E[Player Loses];
    D-->F[/Display message: "You Win!"/];
    E-->G[/Display message: "You Lose!"/];
    F-->H[/Ask Player: "Play again? Y/N" /];
    G-->H[/Ask Player: "Play again? Y/N" /];
    H-- if playAgain = Y -->I[Game Restarts]
    H-- if playAgain = N -->J[Game Ends]
```

1. Game Master rolls a 6 sided die.
2. The player guesses a number between 1 and 6, hoping to match the number that was rolled.
	- If the two numbers match, the player has won the game.
	- If the two numbers do not match, the player has lost the game.
4. The player will be asked if they want to play again.
	- If the player wants to play again, the game restarts.
	- If the player does not want to play again, the game ends.