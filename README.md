Python Blackjack Game
Overview
This is a simple text-based Blackjack game implemented in Python. The game simulates a standard Blackjack game where the player competes against the dealer. It uses the tkinter library for a graphical interface to display the game state.

Features
Text-based user interface.
Full deck of 52 cards with four suits.
Basic Blackjack rules implementation.
Score tracking for both player and dealer.
Player actions: Hit or Stand.
Dealer actions based on standard Blackjack rules.
Handling of special cases like Blackjack and busts.
Gameplay
The player and the dealer are each dealt two cards.
The player can choose to "Hit" (draw another card) or "Stand" (end their turn).
The dealer reveals one of their cards and takes actions according to standard Blackjack rules.
The player wins if they have a higher score than the dealer without exceeding 21.
Special conditions include Blackjack (a score of 21 with two cards) and busts (exceeding a score of 21).
Getting Started
Prerequisites
Python 3.x
The tkinter library (should be included with Python standard library)
Installation
Clone the repository:

sh
Copy code
git clone https://github.com/Mitch002/To-Do-List-App.git
cd To-Do-List-App
Run the blackjack.py script:

sh
Copy code
python blackjack.py
Code Description
The blackjack.py script is divided into several functions and a class:

Card Class
Represents a single card in the deck. Each card has a face value, a numeric value, and a suit symbol.

python
Copy code
class Card:
    def __init__(self, card_face, value, symbol):
        self.card_face = card_face
        self.value = value
        self.symbol = symbol
Functions
show_cards(cards, hidden): Displays the cards on the console.
deal_card(deck): Deals a single card from the deck.
play_blackjack(deck): The main game loop for playing a round of Blackjack.
init_deck(): Initializes a full deck of 52 cards.
Main Script
The main script initializes the deck and starts the game by calling play_blackjack(deck).

python
Copy code
if __name__ == '__main__':
    deck = init_deck()
    play_blackjack(deck)
Example Output
When you run the game, you'll see output similar to this:

yaml
Copy code
PLAYER CARDS:
     ________________     ________________
    |                |   |                |
    |  7             |   |  9             |
    |                |   |                |
    |                |   |                |
    |                |   |                |
    |                |   |                |
    |      ♠         |   |      ♠         |
    |                |   |                |
    |                |   |                |
    |                |   |                |
    |                |   |                |
    |            7   |   |            9   |
    |________________|   |________________|
PLAYER SCORE =  16

DEALER CARDS:
     ________________
    |                |
    |  J             |
    |                |
    |                |
    |                |
    |                |
    |      ♥         |
    |                |
    |                |
    |                |
    |                |
    |            J   |
    |________________|
DEALER SCORE =  10
Contributions
Contributions are welcome! Please feel free to submit a pull request or open an issue to improve the game.
