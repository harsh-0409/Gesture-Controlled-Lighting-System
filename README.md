# Gesture-Controlled Lighting System

A computer vision-based system that controls LED lights using hand gestures. The system detects the number of fingers shown and lights up corresponding LEDs.

## Features

- Real-time hand gesture detection
- Controls 5 LED lights based on finger count
- Supports gestures from 0 to 5 fingers
- Live video feed with gesture recognition feedback

## Technologies Used

- Python 3.x
- OpenCV
- CVZone HandTracking Module
- PyFirmata
- Arduino

## Hardware Requirements

- Arduino board
- 5 LED lights
- Connecting wires
- Webcam

## Software Setup

1. Install required Python packages:
pip install opencv-python

pip install pyfirmata
pip install cvzone


2. Upload StandardFirmata sketch to Arduino board
3. Update COM port in controller.py to match your Arduino port
4. Connect LEDs to digital pins 8-12 on Arduino

## Usage

1. Run the main script:
python new.py


2. Show hand gestures in front of camera:
- 0 fingers: All LEDs off
- 1 finger: First LED on
- 2 fingers: First two LEDs on
- 3 fingers: First three LEDs on
- 4 fingers: First four LEDs on
- 5 fingers: All LEDs on

3. Press 'k' to exit the program

## Code Structure

- `new.py`: Main script with video capture and gesture detection
- `controller.py`: Arduino communication and LED control logic
- `StandardFirmata.ino`: Arduino firmware

## Author

Harsh Raj

## License

This project is licensed under the MIT License - see the LICENSE file for details
