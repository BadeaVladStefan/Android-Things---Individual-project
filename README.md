🕹️ Stop at 5 Seconds – Reaction Timer Game
==========================================

This Arduino project challenges your reflexes!
Your goal is to press the STOP button as close to 5.00 seconds as possible after starting the timer.

📦 What You Need
---------------
- Arduino UNO (or compatible)
- 1602 I2C LCD Display
- 2x Push Buttons
- Jumper Wires - 4 mother-father, 4 father-father
- Breadboard

🔌 Wiring Guide
---------------

🖥️ LCD I2C Display
-------------------
| LCD Pin | Arduino Pin |
|---------|-------------|
| VCC     | 5V          |
| GND     | GND         |
| SDA     | A4          |
| SCL     | A5          |

🔘 Buttons
----------
| Button         | One Leg → | Other Leg → Arduino Pin |
|----------------|-----------|--------------------------|
| Start Button   | GND       | D4                       |
| Stop Button    | GND       | D3                       |

- Use internal pull-up resistors by setting the pins as INPUT_PULLUP in code.
- Make sure buttons are placed across the center gap of the breadboard.

▶️ How to Use
-------------
1. Upload the code to your Arduino.
2. On the LCD, you'll see:
   "Stop at 5 sec!"
   "D4=Start D3=Stop"
3. Press Button D4 to start the timer.
4. The LCD will display:
   "Stop at 5 sec!"
   "Time: 0.00s"
   The time will start counting up.
5. Try to press Button D3 exactly at 5.00 seconds!
6. You'll see your final time:
   "Stopped at:"
   "4.97s"
7. After 2 seconds, the game resets.

