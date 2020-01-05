# Games of chance

* In this interactive Python 3 script, place a bet and play games of dice, a coin toss, and a game of roulette.

## Dice 

* Begin by setting the desired amount to start off betting with. 

* `dice_roll` is the function that checks two conditions are satisfied: the guess is in range of the number of sides on the dice, & the bet is under the `money` amount. 
* If both conditions are satisfied; the guess is checked, if correct, the bet is multiplied by 3. If incorrect, the bet is lost. 


import random
num = random.randint(1, 6)
money = 100 


def dice_roll(guess, bet):
    
    if bet > money or bet <= 0:
        print ("Sorry you can't do that")
        return 0 
    if guess > 6 or guess < 1:
        print ("Pick a number within range of dice")
        return 0 

#now the game starts 
    else:
        print("--------------")
        print("It's time to roll the dice!")
        print ("The number you rolled is " + str(num))

    if guess == num:
        print("--------------")
        print ("You just won " + str(bet*3))
        print("--------------")
        return bet*3

    if guess != num:
        print("--------------")
        print("Sorry you lost -" + str(bet))
        print("--------------")
        return -bet 

dice_roll(4, 10)

## Coin Flip

* `coin_flip` is the function that checks two conditions are satisfied: the guess is correctly **heads** or **tails**, & the bet is under the `money` amount. 
* If both conditions are satisfied; the guess is checked, if correct, the bet is returned. If incorrect, the bet is lost. 

coin flip game

def coin_flip(guess, bet):
    if bet > money:
        print ("Sorry you can't do that")
        return 0 
        
#Now the game starts
    print("--------------") 
    print("The game of coin toss! You chose " + guess + ".")
    result = random.randint(1, 2)

    if result == 1:
        print("Heads!")
    elif result == 2:
        print("Tails!")
    if (guess == "Heads" and result == 1) or (guess == "Tails" and result == 2):
        print("--------------") 
        print("You won {}".format(bet))
        return bet
    else:
        print("--------------") 
        print("You lost {}".format(bet))
        return -bet

#coin_flip("Heads, 10")

## Roulette

* `roulette` is the function that checks two conditions are satisfied: the guess is in range of the number of roulette selections, & the bet is under the `money` amount. 
* If both conditions are satisfied; the guess is checked, if the guess was correct for only even or odd, the bet is returned. If the guess was the correct number exactly, the bet is multiplied by 7.


## Total Money

* The money is added in a running sum based on the guesses and bets from the games.



#compute bets & games played so far
#money += dice_roll(6, 10)
#money += coin_flip("Heads", 50)
#money += roulette("Odd", 40)

#print("Your total amount is $" + str(money))


        
        
