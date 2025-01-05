**Name:**THALAKOKULA SHIVA KUMAR
**Company:**CODTECH IT SOLUTIONS PVT.LTD  
**Intern ID:**CT12DYQ 
**Domain:**Embedded systems *
*Duration:**December 17 to February 17 2025

Overview of the project

## Project : BUILD A BASIC SPEECH RECOGNITION SYSTEM FOR COMMAND-BASED CONTROL OF DEVICES USING AN EMBEDDED BOARD
## Components Required
Embedded board (e.g., Arduino Uno, ESP32, or Raspberry Pi)
Speech recognition module (e.g., Elechouse V3 Voice Recognition Module)
Relay module (to control devices)
Electrical appliances (LED, fan, etc.)
Power supply
Jumper wires
## How It Works
Speech Recognition Module:

Pre-trained to recognize specific voice commands (e.g., "Turn on light", "Turn off fan").
Sends commands to the embedded board.
Embedded Board:

Receives the command via serial communication.
Decodes the command and controls the relays to switch devices on/off.
Relay Module:

Acts as a switch to control high-power devices.
Circuit Diagram
## Connections:
Speech Recognition Module:

VCC → 5V (Arduino or ESP32)
GND → GND
RX → TX (Arduino Pin 2)
TX → RX (Arduino Pin 3)
Relay Module:

IN1 → Pin 8 (Arduino or ESP32)
IN2 → Pin 9
VCC → 5V
GND → GND
Devices:
Connect the positive terminal of the device to the relay's NO (Normally Open) terminal.
Connect the common (COM) terminal to the power source.

## Training Voice Commands
Use the Elechouse Voice Recognition Module V3 or a similar module with a setup tool (usually a GUI) to train commands.
Train commands like:
"Turn on light"
"Turn off light"
"Turn on fan"
"Turn off fan"
Alternative Using ESP32 (Built-In Microphone or External)
If using an ESP32 with TensorFlow Lite Micro:

Train a simple keyword detection model (e.g., "ON", "OFF").
Use TensorFlow Lite Micro or Edge Impulse to deploy a model on the ESP32.
## How It Works
Speech Recognition Module:

Matches spoken commands to pre-trained phrases.
Sends matched command IDs to the board.
Embedded Board:

Maps the command ID to specific device actions.
Relay Module:
Switches devices based on the board's output.

![Screenshot 2025-01-05 125738](https://github.com/user-attachments/assets/abfd2c8a-4656-4fbb-aa28-3ba0a5e87c54)
