# Magical Arena Game

## Overview

This is a simple magical arena game where two players fight until one of them dies. Each player has three attributes: health, strength, and attack. Players attack in turns, rolling dice to determine the amount of damage inflicted and defended.

## Rules

1. Players attack in turns.
2. The player with the lower health attacks first at the start of the match.
3. The attacking player rolls a 6-sided die to determine the attack damage.
4. The defending player rolls a 6-sided die to determine the defense strength.
5. The difference between the attack damage and the defense strength reduces the defender's health.
6. The game ends when a player's health reaches zero.

## Game Mechanics

- **Players**: There are two players, Player A and Player B, each with their own set of attributes (health, strength, attack).
- **Turns**: Players take turns attacking each other based on their current health status.
- **Attacks**: Attacks are determined by rolling a six-sided dice to calculate damage, factoring in the attacker's attack strength and the defender's defense strength.
- **Victory**: The game continues until one player's health drops to zero or below. The player with remaining health wins the match.

## Test Cases

### Player Class Tests

- **testReduceHealth**: Checks if the `reduceHealth` method correctly reduces a player's health and ensures it does not go below zero.
- **testIsAlive**: Tests the `isAlive` method to verify the player's life status based on their current health.

### Arena Class Tests

- **testAttack**: Verifies that the `attack` method correctly reduces the defender's health when an attack is initiated.
- **testStartMatch_PlayerAWins**: Tests the overall match outcome to ensure the correct player is declared the winner based on their remaining health.
- **testRollDice**: Validates the `rollDice` method to ensure it produces results within the expected range (1 to 6).


## How to Run

1. Clone the repository.
2. Open the project in your favorite IDE.
3. Run the `Main` class to start the game.
4. To run the unit tests, use your IDE's built-in testing tools or run `mvn test` if using Maven.






