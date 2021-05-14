# RL_based_Tic-Tac-Toe
In this project, we built an RL agent that learns to play Numerical Tic-Tac-Toe with odd numbers assuming that the player will play first. The project is without any UI but has the backend functionality that is used in the Tic-Tac-Toe game.

In this project, instead of X’s and O’s, the numbers 1 to 9 are used. In the 3x3 grid, numbers 1 to 9 are filled, with one number in each cell. The first player plays with the odd numbers, the second player plays with the even numbers, i.e. player 1 can enter only an odd number in the cell while player 2 can enter an even number in one of the remaining cells. Each number can be used exactly once in the entire grid. The player who puts down 15 points in a line - (column, row or a diagonal) wins the game. 

**RULES OF THE GAME:**
1) The game will be played on a 3x3 grid (9 cells) using numbers from 1 to 9. Each number can be used exactly once in the entire grid.

2) There are two players: one is the Reinforcement Learning (RL) agent and other is the environment.

3) The RL agent is given odd numbers {1, 3, 5, 7, 9} and the environment is given the even numbers {2, 4, 6, 8}

4) Each of them takes a turn. The player with odd numbers always goes first.

5) At each round, a player puts one unused number on a blank spot.

6) The objective is to make 15 points in a row, column or a diagonal. The player can use the opponent's numbers in the grid to make 15.

7) The game terminates when any one of the players makes 15.

We have trained agent using Q-Learning. The environment is playing randomly with the agent, i.e. its strategy is to put an even number randomly in an empty cell. 
If your agent wins the game, it gets 10 points, if the environment wins, the agent loses 10 points. And if the game ends in a draw, it gets 0. Also, you want the agent to win in as few moves as possible, so for each move, it gets a -1 point.

The accuracy of the model is checked by whether Q-values learnt by the agent have converged or not.

That can be found by the plot given at the end.

No dataset is used in this project as the numbers are generated randomly and the learning is done using Reinforcement Learning models.
