UNO BANK – Python Card Game

A fun, logic-based money survival card game with Single-Player and Two-Player Modes

📌 Overview
Uno Bank is a beginner-friendly yet exciting Python card game where your goal is simple:
Survive the deck and finish with the highest bank balance!
You start with $10 and 10 draws.
Each draw reveals a card that affects your money or draw count.
In 2-Player Mode, new yellow cards introduce competitive twists like stealing, swapping, bombing, and transferring balances.

This project is great for practicing:
✔ Randomization
✔ Loops & condition handling
✔ Functions
✔ Multi-player logic
✔ Terminal-based gameplay

🎮 Game Modes
1️.Single Player Mode
Start with $10 and 10 draws
Draw cards one by one
Cards affect:
your balance (+ / – money)
your remaining draws
your balance multiplier (x2 or /2)
Game ends when draws reach 0
Shows final balance

2️. Two-Player Mode
Both players start with $10 and 10 draws
Players take turns drawing cards
Includes new Yellow Cards that affect opponents
Game ends when any player runs out of draws
Player with the higher balance wins

🃏 Card Types & Effects
Green Cards (Money Gain)
Card	Effect
+1	Add $1
+3	Add $3
+5	Add $5
+7	Add $7
Blue Cards (Money Loss)
Card	Effect
-2	Subtract $2
-4	Subtract $4
-6	Subtract $6
-8	Subtract $8
Black Cards (Special Effects)
Card	Effect
x2	Double your balance
/2	Halve your balance
+2D	Gain 2 draws
-2D	Lose 2 draws
🟡 Yellow Cards (Two-Player Mode Only)
Card	Effect
SWAP	Swap balances with opponent
FORWARD	Give all your money to opponent
BACKWARD	Steal all opponent's money
BOMB	Reset your balance to $0

🛠 Installation & Requirements
Requires Python 3.8+
No external libraries — only built-in modules:
random  
time  


To run the game:
python main.py
▶ How to Play

Run the program
Choose Single Player or Two Player
Follow the prompts
Draws reduce automatically
For 2 players → alternate turns
Game ends when draws = 0
Winner is announced

📂 Project Structure
UnoBank/
│
├── main.py             # Entire game logic (single + two player)
└── README.md           # Game documentation

✨ Features
✔ Clean text-based UI
✔ Random card draws
✔ Money management logic
✔ Multi-player mode with interactions
✔ Balance effects & draw mechanics
✔ Beginner-friendly and expandable

🚀 Future Enhancements
Tkinter GUI version
Pygame animated version
Sound effects
Scoreboard & history
Online multiplayer
