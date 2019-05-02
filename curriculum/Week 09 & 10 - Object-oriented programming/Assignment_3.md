# Dice Poker

## RULES OF THE GAME

- The player starts with $100.
- Each round costs $10 to play. This amount is subtracted from the player’s money at the start of the round.
- The player initially rolls a completely random hand (i.e., all the five dice are rolled).
- The player gets two chances to enhance the hand by rerolling some or all of the dice.
- At the end of the hand, the player’s money is updated according to the following payout schedule:

| Hand | Pay |
| --- | --- |
| Two Pairs | 5 |
| Three of a Kind | 8 |
| Full House | 12  |
| Four of a Kind | 15 |
| Straight | 20 |
| Five of a Kind | 30 |


## Explanation of the scoring
Two pairs is two sets of pairs, for example two threes and two eights in the same hand.
A Full House is a pair and a Three of a Kind in the same hand.  
Four of a kind is four of the same card, such as four eights.
A straight is five numbers in order. So this can be 12345 or 23456.
Five of a kind are five of the same number (all sixes for example).

## Instructions

Build a Dice Poker game according to the game rules above. Ultimately, we want this program to present a nice graphical interface. Our interaction will be through mouse clicks. The interface should have the following characteristics:

- The current score (amount of money) is constantly displayed.
- The program automatically terminates if the player goes broke.
- The display may choose to quit at appropriate points during play.
- The interface will present visual cues to indicate what is going on at any given moment and what the valid user responses are.

This class has to implement these operations:
1.	Constructor - Create the initial collection.
2.	Roll - Assign a random value to some subset of the dice while maintaining the current value of others.
3.	Value - return the current values of the five dice.
4.	Score - return the score for the dice.
