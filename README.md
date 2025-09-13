# Arduino Pedestrian Crossing System

This Arduino project implements a pedestrian crossing system with visual indicators using an LCD display and LED lights. Here's what the code does:

## Components:
- I2C LCD display (16x2 characters)
- Three LEDs (green, orange, red)
- One push button

## Functionality:

1. **Normal State (Button Not Pressed)**:
   - Green LED is on
   - LCD displays "VEHICLES GO" and "WAIT TO CROSS"
   - Vehicles have right of way

2. **When Button is Pressed**:
   - System detects pedestrian waiting
   - Orange LED turns on
   - LCD shows a 5-second countdown with "PEDESTRIAN WAITING"

3. **After Countdown**:
   - Red LED turns on (orange turns off)
   - LCD shows a 15-second countdown with "PEDESTRIAN CROSSING"
   - Pedestrians can safely cross

4. **After Crossing Period**:
   - Red LED turns off
   - Orange LED blinks once
   - System returns to normal state (green LED on)

The system provides both visual feedback through the LEDs and detailed information on the LCD display, making it clear to both drivers and pedestrians what the current state is.
