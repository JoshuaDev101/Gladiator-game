****Gladiator1 Game
****This is a simple turn-based gladiator fighting game written in Java. The game allows you to create a player gladiator and automatically generate a computer-controlled enemy gladiator. Both gladiators fight until one wins.
Features
- Gladiator Class (Gladiator1)
  * Attributes: name, health, damage, defense, initiative
  * Validation for each attribute (health > 0, damage > 0, etc.)
  * Getter and setter methods
  * fight() method that simulates a battle between two gladiators
  * displayGladiatorStats() to show gladiator details before the fight

- Game Class (GladiatorGame)
  * Prompts the user to enter their gladiator’s stats
  * Creates a computer-controlled enemy with randomized stats
  * Calls the fight() method to simulate the battle
  * Displays the winner at the end
How to Run
1. Save the files in the following structure:
   Gladiator_java/
   └── src/
       ├── Gladiator1.java
       └── GladiatorGame.java

2. Make sure the first line in both files matches the package:
   package src;

3. Compile the classes from the Gladiator_java/src folder:
   javac src/Gladiator1.java src/GladiatorGame.java

4. Run the game:
   java src.GladiatorGame
Example Gameplay
Enter Gladiator 1 Name: Maximus
Enter Maximus health points: 120
Enter Maximus damage points: 40
Enter Maximus defense points: 20
Enter Maximus initiative: 50

Maximus, health: 120.0, damage: 40, defense: 20, initiative: 50
Computer, health: 100.0, damage: 32, defense: 18, initiative: 65

Round 1: Computer does 32 damage 20% of which Maximus ignores. Maximus has 94.4 health left.
Round 2: Maximus does 40 damage 18% of which Computer ignores. Computer has 67.2 health left.
...

Computer wins.
Notes
- Initiative decides who attacks first.
- Defense reduces the effective damage taken.
- Battle continues until one gladiator’s health drops to 0 or below.
- User input is validated (e.g., negative values are not allowed).
OOP Concepts
This project is a good introduction to Object-Oriented Programming (OOP) in Java with concepts like:
- Classes and Objects
- Encapsulation (private fields + getters/setters)
- Static methods
- Loops and conditionals
