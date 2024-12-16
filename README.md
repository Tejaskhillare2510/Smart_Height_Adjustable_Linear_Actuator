# Smart_Height_Adjustable_Linear_Actuator
The height of the linear actuator can be controlled using the ESP32.
**Overview**
The project aims to design a smart table whose height can be adjusted automatically using voice commands. The system leverages ESP32, linear actuators, and feedback sensors to control the table's position precisely.

**The project evolved through two prototypes:**

Prototype 1: Time-based relay control without feedback.
Prototype 2: Enhanced with an ultrasonic sensor for precise height control and Google Assistant integration via Arduino Cloud.
Features
Voice Control: Adjust the table height using Google Assistant.

Feedback Mechanism: Ultrasonic sensors provide real-time height monitoring.

Manual Control: Button-operated control for manual height adjustment.

IoT Integration: Remote monitoring and control using the Arduino Cloud.

**System Components**
Hardware Used
ESP32 Microcontroller
Linear Actuators
Relay Module
Ultrasonic Sensor (for height feedback)
Push Buttons (for manual control)
Power Supply (12V/24V for actuators)
Software Tools
Arduino IDE: For ESP32 programming
Google Assistant: Integrated via Arduino Cloud
SolidWorks: For 3D design of the table case
Altium Designer: For PCB design
Arduino Cloud: IoT dashboard and integration


**System Architecture**

**Circuit Diagram**
![image](https://github.com/user-attachments/assets/d66e65c4-ccd3-432a-94be-10a2d092e81c)


**How It Works**
**Step 1: Control Mechanism**
Google Assistant sends voice commands to the Arduino Cloud.
The ESP32 microcontroller receives height commands via Wi-Fi.
**Step 2: Actuator Operation**
The relay module triggers the linear actuators to move up or down.
Ultrasonic sensors continuously monitor the table height.
**Step 3: Feedback & Monitoring**
Real-time height data is sent to the Arduino Cloud for monitoring.


**Prototypes**
**Prototype 1: Time-Based Relay Control**
Linear actuators were controlled without feedback.
IFTTT integration allowed only basic text commands, limiting flexibility.
**Prototype 2: Enhanced Feedback Control**
Ultrasonic sensors were used for accurate height feedback.
Google Assistant integration was improved using Arduino Cloud.


**Schematics and Designs**

**Schematics Diagram**

![image](https://github.com/user-attachments/assets/496421e3-2308-4ec0-b09e-8da5c8bbd27f)

**PCB Design**

![image](https://github.com/user-attachments/assets/0cea1fb0-dc7c-417a-8f2a-d7b233bafffc)

![image](https://github.com/user-attachments/assets/5f1b11b0-cf9a-487d-bca9-9ccb74e27e91)

**3D Table Case Design**

![image](https://github.com/user-attachments/assets/d55c4954-7412-41b5-9f31-12df0e1a916f)


**Main Code Features :**
Google Assistant Integration via Arduino Cloud
Manual Height Adjustment
Feedback Mechanism with Ultrasonic Sensor
To upload the code to ESP32:

**Hardware Setup:**
Connect ESP32, relay module, linear actuators, and ultrasonic sensor as per the circuit diagram.

**Software Configuration :**
Flash the ESP32 with the code provided.
Configure Google Assistant with Arduino Cloud.

**Testing:**
Use voice commands like "Hey Google, set table height to 40 cm."
Monitor the height feedback through the Arduino Cloud dashboard.
Images and Media
System Images

Google Assistant Demo

**Future Improvements :**
Integration with Machine Learning for smarter height adjustments based on user preferences.
Addition of safety features like collision detection.
Expansion to other voice assistants (Alexa, Siri).

