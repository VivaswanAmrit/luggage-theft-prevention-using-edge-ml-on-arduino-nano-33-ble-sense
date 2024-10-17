# luggage-theft-prevention-using-edge-ml-on-arduino-nano-33-ble-sense

Motion Detection System to Prevent Luggage Theft
Project Overview

This project focuses on building a motion detection system designed to prevent luggage theft. 
Using Edge Impulse to train an Edge AI model, I deployed the solution on an Arduino Nano 33 BLE Sense board with an accelerometer to detect abnormal movements 
and raise an alert when potential theft is detected.

Features
Motion Detection: Monitors luggage for suspicious movements using onboard accelerometer data.
Edge Deployment: The AI model runs locally on the Arduino Nano 33 BLE Sense, enabling real-time theft prevention without the need for cloud connectivity.
Customizable Sensitivity: Sensitivity settings can be adjusted to reduce false alarms based on specific conditions, such as handling vs. theft.

Getting Started
Prerequisites
Arduino Nano 33 BLE Sense board.
Edge Impulse account and tools.
Arduino IDE installed on your computer.
Buzzer or LED (optional) for alert notifications.

Hardware Setup
Arduino Nano 33 BLE Sense is equipped with a built-in accelerometer to track movement.
Connect optional components such as a buzzer or LED to serve as an alarm when motion is detected.

Software Setup
Train the Model on Edge Impulse:

Collect accelerometer data from normal and suspicious movements.
Label data for different scenarios (e.g., stationary, handling, theft-like motion).
Use Edge Impulse to train a model to classify motion into normal vs. abnormal categories.
Deploy the Model:

After achieving good accuracy, download the Arduino Library from Edge Impulse.
Install the library into the Arduino IDE.
Use the pre-built example code from the library to load the model onto the Arduino Nano 33 BLE Sense.
The model will now monitor for abnormal movements in real time and trigger an alert when suspicious activity is detected.

Model Details
Training Data: Collected from accelerometer readings during both normal handling and theft scenarios.
Labels:
Normal Movement (e.g., casual handling, picking up).
Suspicious Movement (e.g., rapid or unexpected movement consistent with theft).
Deployment: Model runs in real-time on the Arduino Nano 33 BLE Sense.
Usage Instructions
Attach the Arduino Nano 33 BLE Sense to your luggage.
The device will monitor movement patterns, and if it detects abnormal or suspicious motion, it will trigger an alert (buzzer or LED).
Sensitivity can be fine-tuned to differentiate between normal handling and potential theft behavior.

Future Improvements
Incorporate a mobile notification system for remote alerts via Bluetooth or Wi-Fi.
Expand the model to classify additional behaviors (e.g., dragging, jostling).
Optimize for battery life, enabling longer periods of unattended operation.
