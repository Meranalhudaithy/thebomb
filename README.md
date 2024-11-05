# 💣 Defuse the BOMB Game 🎮

Welcome to **Defuse the Bomb**, a two-player Arduino-based game that challenges players to disarm a simulated bomb before time runs out. It combines teamwork, quick thinking, and a bit of suspense to create a thrilling interactive experience. 

---
## 👥 Contributors

Thanks to everyone who has contributed to this project!

- Meran Alhudaithy (https://github.com/Meranalhudaithy) 
- Ahmed Aldayel   (https://github.com/ahDayel) 


---

## 📋 Project Overview
In **Defuse the Bomb**, one player acts as the **Defuser**, working against a countdown to deactivate the bomb, while the other player, the **Assistant**, provides critical guidance using a defusal guide. This game is a blend of logic, teamwork, and timing – perfect for anyone looking to explore interactive electronics and game development with Arduino!

---

## 🛠 Hardware Requirements

To bring this project to life, you'll need:

- **Arduino Uno** (or a compatible board)
- **I2C LCD Display (16x2)** - Displays the countdown and game messages
- **7-Segment Display** - Shows the timer for added suspense
- **LEDs**:
  - Red
  - Yellow
  - Green
- **Pushbuttons** - For in-game interactions
- **Resistors** - Various values for current limiting
- **Breadboard** - For assembling components
- **Jumper Wires** - For connecting everything together

---

## 🎯 Game Objective
The goal is simple: **Defuse the bomb before the timer hits zero!** The Defuser must carefully follow instructions from the Assistant, who uses the defusal guide based on symbols displayed on the LCD. Each symbol represents a unique defusal challenge, making every playthrough different and exciting.

---

## 🔥 Game Features

- **Countdown Timer**: A 7-segment display shows the time ticking down, adding urgency to the gameplay.
- **LED Indicators**: Red, yellow, and green LEDs provide visual cues to track progress or signal mistakes.
- **Random Defusal Scenarios**: The game selects different defusal scenarios, keeping each session unique.
- **Strike System**: Two mistakes lead to a game-over, simulating an "explosion."

---

## 🕹 How to Play

1. **Starting the Game**:
   - The Defuser presses a button to start the countdown.
   - A symbol appears on the LCD screen, guiding the Assistant to find the defusal steps.

2. **Defusing Process**:
   - The Assistant reads instructions based on the symbol and provides them to the Defuser.
   - The Defuser follows these steps by pressing buttons and observing the LEDs to ensure the correct sequence.
   - If successful, the LCD displays **"BOMB DEFUSED!"** If unsuccessful, the display reads **"BOOM!"**

3. **Winning and Losing**:
   - Disarm the bomb before time expires to win.
   - Fail by either running out of time or accumulating two strikes, resulting in a simulated "explosion."

---

## 🚀 Installation Steps

### Step 1: Hardware Setup
Follow these steps to assemble the hardware components:

1. **Connect the LCD Display**: 
   - Wire the I2C LCD display to the Arduino, connecting the SDA and SCL pins to the corresponding Arduino pins.

2. **Set Up the LEDs**:
   - Connect each LED (red, yellow, green) to digital pins on the Arduino.
   - Add resistors between each LED and ground to prevent overcurrent.

3. **Attach the 7-Segment Display**: 
   - Connect the 7-segment display to the appropriate Arduino pins following the code’s pin mapping.

4. **Connect the Buttons**:
   - Place the pushbuttons on the breadboard and connect them to input pins on the Arduino with pull-down resistors.

![The Bomb Simulation](https://github.com/user-attachments/assets/5da790fb-21a1-4369-b63c-29399f424dd7)

---

### Step 2: Code Setup

1. **Download the Code**:
   - Access the code from the main branch of the repository (e.g., `ArduinoCode` file).
   - Copy or download the code and open it in the Arduino IDE.

2. **Upload the Code**:
   - Connect your Arduino to your computer and upload the code to the board.

3. **Power Up**:
   - Once the code is uploaded, power up the Arduino. The LCD screen will display the initial game message.

---

### Step 3: Defusal Guide 📝

**Defusing Guide**: Each symbol displayed on the LCD corresponds to a unique set of defusal instructions. Use the guide to interpret these symbols and help the Defuser complete the sequence. Here’s an example:

![image](https://github.com/user-attachments/assets/5fe8fbc3-0437-4c5d-a594-06f970555e09)


- **Symbol: o7** - Specific LED order and conditions.
- **Symbol: ^^, ^^** - Count red-yellow and red-green light overlaps.
- **Symbol: <3** - True/False questions about light status.

---

## 📜 License

This project is open-source and free for personal and educational use. Feel free to modify, share, and enjoy!

Enjoy the challenge and test your teamwork, problem-solving, and Arduino skills with **Defuse the Bomb**! Good luck, and don’t let it blow up! 💥

