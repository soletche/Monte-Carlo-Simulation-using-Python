# Monte-Carlo-Simulation-using-Python
Walkthrough an example to learn what a Monte Carlo simulation is and how it can be used to predict probabilities

When learning how to build Monte Carlo simulations, it’s best to start with a basic model to understand the fundamentals. The easiest and most common way to do that is with simple games, so we will make use of a dice game in this article. You’ve probably heard the saying, “the house always wins,” so for this example, the house (typically a casino) will have an advantage, and we will show what that means for the player’s possible earnings.

# The Dice Game

Our simple game will involve two six-sided dice. In order to win, the player needs to roll the same number on both dice. A six-sided die has six possible outcomes (1, 2, 3, 4, 5, and 6). With two dice, there is now 36 possible outcomes (1 and 1, 1 and 2, 1 and 3, etc., or 6 x 6 = 36 possibilities). In this game, the house has more opportunities to win (30 outcomes vs. the player’s 6 outcomes), meaning the house has the quite the advantage.

Let’s say our player starts with a balance of $1,000 and is prepared to lose it all, so they bet $1 on every roll (meaning both dice are rolled) and decide to play 1,000 rolls. Because the house is so generous, they offer to payout 4 times the player’s bet when the player wins. For example, if the player wins the first roll, their balance increases by $4, and they end the round with a balance of $1,004. If they miraculously went on a 1,000 roll win-streak, they could go home with $5,000. If they lost every round, they could go home with nothing. Not a bad risk-reward ratio… or maybe it is.

The most important part of any Monte Carlo simulation (or any analysis for that matter) is drawing conclusions from the results. From the figure of the code, we can determine that the player rarely makes a profit after 1,000 rolls. In fact, the average ending balance of our 10,000 simulations is $833.66 (your results may be slightly different due to randomization). So, even though the house was “generous” in paying out 4 times our bet when the player won, the house still came out on top.

![imagen](https://github.com/soletche/Monte-Carlo-Simulation-using-Python/assets/114614816/0c1dc93e-e8cb-4fbe-aa57-77c34a9fe3b7)

![imagen](https://github.com/soletche/Monte-Carlo-Simulation-using-Python/assets/114614816/878e28dd-c1fa-401e-a34f-fa069fa2c1a5)

Noted that the player had 6 outcomes in which they could win. We also noted there are 36 possible rolls. Using these two numbers, we would expect that the player would win 6 out of 36 rolls, or 1/6 rolls, which matches our Monte Carlo prediction.
