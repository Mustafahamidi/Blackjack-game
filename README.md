# Blackjack Game

A simple Blackjack game implemented in JavaScript. This project is a basic simulation of the popular card game Blackjack, where the goal is to get a hand value as close to 21 as possible without going over.

## How It Works

The game includes the following features:
- A player object with a name and starting chips.
- Random card generation with values adjusted for face cards and Aces.
- Basic game logic to determine if the player has Blackjack, is still in the game, or has busted.
- Dynamic updates to the DOM to display the player's cards, sum, and game messages.

### Game Rules
1. The game starts by dealing two random cards to the player.
2. The player can choose to draw a new card (`newCard`) to add to their hand.
3. If the player's hand sum exceeds 21, they lose (bust).
4. If the player's hand sum equals 21, they win (Blackjack).
5. The player can choose to stop drawing cards at any time.

## Code Structure

- **Player Object**: Tracks the player's name and chip count.
- **Cards Array**: Stores the player's current hand.
- **Game Logic**:
  - `getRandomCard()`: Generates a random card value between 1 and 11.
  - `startGame()`: Initializes the game by dealing two cards and calculating the sum.
  - `renderGame()`: Updates the DOM to display the current cards, sum, and game status.
  - `newCard()`: Allows the player to draw an additional card if they are still in the game.

## How to Use

1. Clone the repository or download the code.
2. Open the `index.html` file in your browser.
3. Interact with the game using the provided buttons:
   - **Start Game**: Deals the initial two cards.
   - **New Card**: Draws an additional card (if the game is still active).

## Example

```javascript
let player = {
    name: "Mustafa",
    chips: 120
};

// Start the game
startGame();

// Draw a new card (if the game is still active)
newCard();
