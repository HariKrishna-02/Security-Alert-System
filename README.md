# Security-Alert-System

The Security Alert System is a simple and effective project using an Arduino Uno and a PIR motion sensor. It detects movement based on body heat within about 15-20 feet. When motion is detected, the sensor sends a signal to the Arduino, which instantly activates an LED light and buzzer for one second to alert and scare intruders.

The main components include the Arduino Uno board, HC-SR501 PIR sensor, LED, buzzer, connecting wires, and power supply. The PIR sensor has a Fresnel lens to focus infrared radiation and pyroelectric sensors to detect heat changes. It can be adjusted for sensitivity and trigger duration.

This system works 24/7 without needing internet, so it's reliable and hard to hack. It can be used to protect homes, offices, garages, and storage areas affordably. The design helps reduce false alarms by distinguishing humans from small animals. The system is easy to build and can be enhanced with features like SMS alerts or multiple sensors.

This project serves as a basic, low-cost security guard that provides instant visual and audio alerts when intrusion is detected, making it ideal for beginners wanting home or office protection using simple electronic parts.

# Materials Required

1.ESP32 development board (controls the system, has Wi-Fi/Bluetooth)
2.HC-SR501 PIR motion sensor (detects human movement via heat)
3.LED (visual alert)
4.Active buzzer (audible alarm)
5.Breadboard or PCB (for circuit assembly)
6.Jumper wires (for connections)
7.3.3V power source (ESP32 operates at 3.3V, can be USB or LiPo battery)
8.Resistors (220 ohm for LED)
9.USB cable (for programming and powering ESP32)

Procedure

Step 1: Gather all components you need — ESP32 board, PIR sensor, buzzer, LED, jumper wires, breadboard, and power source.

Step 2: Connect the PIR sensor’s VCC to ESP32’s 3.3V pin, GND to GND, and the sensor’s output pin to a digital GPIO pin on ESP32 (e.g., GPIO 23).

Step 3: Connect the LED’s anode through a 220Ω resistor to a digital GPIO pin (e.g., GPIO 18), and its cathode to GND.

Step 4: Connect the buzzer’s positive terminal to a GPIO pin (e.g., GPIO 19) and the negative terminal to GND.

Step 5: Power the ESP32 via USB or a suitable 3.3V source ensuring stable power supply.

Step 6: Write your code in Arduino IDE. The code should read PIR sensor input; when motion is detected (HIGH), turn ON LED and buzzer for 1 second then turn them OFF.

Step 7: Upload the code to ESP32 using the Arduino IDE.

Step 8: Test your system by moving in front of the PIR sensor; the LED should light up and the buzzer sound for one second.

Step 9: Once tested, install the system in the desired location ensuring components are secured and protected from dust or damage.

Step 10 (Optional): Enhance the project by adding features like Wi-Fi notifications to your phone with ESP32’s wireless capabilities.

Contributing:

We welcome contributions to this project! If you have suggestions, improvements, or bug fixes, please submit a pull request. You're also encouraged to open issues for discussions or to propose new features.
