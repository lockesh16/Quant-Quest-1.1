# Quant-Quest: 1.1
Link to competition: https://quant-quest.auquan.com/problem/problem1 <br/> 
Solution to the problem of Quant Quest Challenge 1 conducted by Auquan <br/>
## PROBLEM STATEMENT: To roll or not to roll? <br/>
You are playing a game with a n-sided fair die. After your first roll, you have a choice to either get paid the face value of the roll, or pay one dollar and roll again. You can continue to do this till you decide to stop. You need to calculate the expected value of this game <br/><br/>
So for a 6 sided die, assume the first roll is 2. You can either get paid $2 and stop playing or pay $1 and roll again. If you choose to roll again and the next roll is 4. If you stop playing now, you earn $3 ($4 - $1), or you can choose to pay $1 more, and continue. What is the expected value of the game, if you were to play it optimally. <br/>
#### INSTRUCTIONS <br/>
1) Work out the logic to calculate the expected value of the game.
2) Code your logic and submit a file (in Python) which contains your code. It should have one function getExpectedValue(int n), which takes an integer input n, and outputs the expected value for the n-sided fair die.
3) Your solution should be a math function. Solving the question by running simulations is not allowed <br/>
# SOLUTION <br/>
No. of faces in dice: **N** <br/><br/>
Let us say we have some **x** between 1 to N, where we stop at first roll only we have output of the roll greater than **x**. <br/><br/>
If output is less than **x**, then we move to next roll by paying one rupee. Now if we forget our previous steps for a moment, we can see that we are at the same position where we were at the first roll i.e. we will stop at second roll if output is greater than x or we will move on to next step. <br/><br/>
Assuming expected value of this game is **E**, we can safely write:<br/><br/>
E = [(N-x)/N\*(x+N+1)/2 + x/N\*(E-1)] 



