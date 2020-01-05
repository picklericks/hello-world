# Games of chance

* In this interactive Python 3 script, place a bet and play games of dice, a coin toss, and a game of roulette.

## Dice 

* Begin by setting the desired amount to start off betting with. 
* `dice_roll` is the function that checks two conditions are satisfied: the guess is in range of the number of sides on the dice, & the bet is under the `money` amount. 
* If both conditions are satisfied; the guess is checked, if correct, the bet is multiplied by 3. If incorrect, the bet is lost. 

## Coin Flip

* `coin_flip` is the function that checks two conditions are satisfied: the guess is correctly **heads** or **tails**, & the bet is under the `money` amount. 
* If both conditions are satisfied; the guess is checked, if correct, the bet is returned. If incorrect, the bet is lost. 

## Roulette

* `roulette` is the function that checks two conditions are satisfied: the guess is in range of the number of roulette selections, & the bet is under the `money` amount. 
* If both conditions are satisfied; the guess is checked, if the guess was correct for only even or odd, the bet is returned. If the guess was the correct number exactly, the bet is multiplied by 7.


## Total Money

* The money is added in a running sum based on the guesses and bets from the games.




        
        
