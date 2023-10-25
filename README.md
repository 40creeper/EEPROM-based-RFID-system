Project Report: RFID-Based Door Access Control System
Table of Contents
Project Overview
Objective
Hardware Components
Software Components
System Architecture
Functionalities
User Guide
Results
Challenges and Limitations
Future Improvements
Conclusion
References
1. Project Overview
The RFID-Based Door Access Control System is an embedded system that utilizes RFID (Radio-Frequency Identification) technology to control access to a secured area or a door. The system consists of an ESP8266 microcontroller, an RFID module, a 16x2 LCD display, and a web server. Users are required to authenticate using a web-based interface before being granted access.

2. Objective
The main objective of this project is to create a secure and user-friendly access control system that provides controlled access to a specific area. The system should be able to:

Allow authorized users to unlock the door using their RFID cards.
Maintain a list of authorized users and their RFID card information.
Allow administrators to add or remove users through a web interface.
Provide a secure login mechanism for administrators to manage the system.
3. Hardware Components
The following hardware components are used in the project:

ESP8266 WiFi module
MFRC522 RFID module
16x2 I2C LCD display
Electronic lock mechanism
Buzzer
LEDs
Breadboard and connecting wires
4. Software Components
The software components used in the project include:

Arduino IDE for programming the ESP8266 microcontroller.
Libraries such as Wire, MFRC522, LiquidCrystal_I2C, ESP8266WiFi, and ESP8266WebServer.
Google Apps Script for cloud-based data storage.
HTML and CSS for creating web interfaces.
5. System Architecture
The system follows a client-server architecture:

The ESP8266 microcontroller serves as the client and controls the hardware components.
The Google Apps Script acts as a server to store and manage authorized user data.
The web server running on the ESP8266 microcontroller provides a user interface for administrators and communicates with the Google Apps Script server.
6. Functionalities
The RFID-Based Door Access Control System offers the following functionalities:

RFID card authentication for access control.
Web-based user interface for administrators to manage users.
Real-time feedback through the 16x2 LCD display.
Audible feedback using a buzzer.
LED indicators for system status.
Secure user authentication for administrators.
Ability to add, remove, and view authorized users.
7. User Guide
For Administrators:
Connect to the system's WiFi network.
Open a web browser and navigate to the system's IP address (default: http://<ESP8266_IP>/).
Log in with the provided username and password.
Add or remove users as needed.
For Users:
Present an authorized RFID card to the RFID module.
The system will either grant or deny access and provide visual and audible feedback.
8. Results
The RFID-Based Door Access Control System successfully provides access control based on RFID card authentication. Administrators can easily manage user access through a web interface, and the system provides real-time feedback to users.

9. Challenges and Limitations
Limited storage capacity: The EEPROM storage of the ESP8266 has a limited capacity for storing user data.
Security: While the system offers basic security for administrators, further security measures can be implemented.
Scalability: The system may require additional features for scalability in larger environments.
10. Future Improvements
Implement a database for more extensive storage of user data.
Enhance security features, such as multi-factor authentication.
Enable remote access and control via a mobile app.
Integrate with a cloud-based authentication service for user management.
11. Conclusion
The RFID-Based Door Access Control System provides a secure and user-friendly solution for access control. It can be used in various applications, including homes, offices, and industrial facilities, to ensure authorized access to secured areas.

12. References
ESP8266 WiFi Module
MFRC522 RFID Module
Arduino IDE
Google Apps Script
LiquidCrystal_I2C Library
ESP8266WiFi Library
ESP8266WebServer Library
