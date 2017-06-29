# Card-Counting

You will write a card counting function. It will receive a card parameter and increment or decrement the global count variable according to the card's value (see table). The function will then return a string with the current count and the string "Bet" if the count is positive, or "Hold" if the count is zero or negative. The current count and the player's decision ("Bet" or "Hold") should be separated by a single space.

Code Explanation:

Check the value of each card via a switch statement.
The variable count:
Increases by 1 if the card is a 2, 3, 4, 5, or 6.
Since 7, 8, and 9 aren't worth anything, we ignore those cards in our switch statement.
Decreases by 1 if the card is a 10, 'J', 'Q', 'K', or 'A'.
Check the value of count and return the appropriate response.
Example Run

cc(2); runs.
The switch statement hits case 2, jumps down and adds 1 to the variable count.
The switch statement then hits the break and cc(3); runs.
This cycle continues until the final call is made, cc('A');.
After the switch statement, the if statement checks count, which is now 0.
This then drops down to the else statement, which will return 0 Hold.
Note: As mentioned earlier, the switch statement could have also been an else if statement.
