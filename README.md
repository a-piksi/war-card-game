# war-card-game
An implementation of a card game "War" for Module 1, Sprint 3, Part 3

## Task description
Create a program, which implements a classic card game "War" for two players.

The rules of the game:
- The objective of the game is to win all the cards.
- All 52 playing cards (without Jockers) are shuffled and divided evenly among the players, giving each a down stack.
- Each player simultaneously draws a card face up, always from the top of the deck. This is called a "battle".
- Then the players compare placed cards by their rank (low -> high: 2, 3, 4, 5, 6, 7, 8, 9, 10, J, Q, K, A) and suits are ignored.
- A card with the highest rank wins and the winner takes both cards, shuffles them and adds to the bottom of the deck.
- If the ranks of the cards are equal, then there is "war" - both players place their next card face down and then another card face up.
- Winning rules apply as before - player with the highest face up card wins the war, shuffles all played cards and adds them to the bottom of their deck.
- If the face up cards are again equal then the battle repeats with another set of face down/up cards. This repeats until one of the face up cards are higher than the other.
- If a player has to play their last card face down, they instead play it face up for the reminder of the war, until someone wins.
- The game ends when one of the players collects all cards and becomes a winner.

The requirements for the program:
- Create a class "Player", which represents each player and implement player moves and actions as methods.
- Create a class "Cards", which represents 52 playing cards and their methods.
- Generate a deck of 52 cards as a list in a randomized order.
- Shuffle the cards in a random order and split them into two even decks.
- Assign those decks to each player. The first card in the list is the first card on top of a player's deck.
- Prompt user's to press a ENTER to start and see next move. Each move is a draw of cards from each player's decks according to rules.
- Implement logic for a "battle"
- Implement logic for a "war"
- All played cards should be returned to the winner in a randomized order, to the bottom of the deck.
- Print the visualization of each move. Face down cards should not be revealed, unless it is the last card. 
- Declare who won after every "battle" and "war".
- When game ends, declare the winner and quit the program.
