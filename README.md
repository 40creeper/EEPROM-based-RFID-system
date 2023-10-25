<!DOCTYPE html>
<html>
<head>
    <title>Project Report: RFID-Based Door Access Control System</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
        }
        h1 {
            text-align: center;
        }
        h2 {
            margin-top: 20px;
        }
        h3 {
            margin-top: 10px;
        }
        ul {
            margin-bottom: 10px;
        }
        ol {
            margin-bottom: 10px;
        }
    </style>
</head>
<body>
    <h1>Project Report: RFID-Based Door Access Control System</h1>

   <h2>Table of Contents</h2>
    <ol>
        <li><a href="#section1">Project Overview</a></li>
        <li><a href="#section2">Objective</a></li>
        <li><a href="#section3">Hardware Components</a></li>
        <li><a href="#section4">Software Components</a></li>
        <li><a href="#section5">System Architecture</a></li>
        <li><a href="#section6">Functionalities</a></li>
        <li><a href="#section7">User Guide</a></li>
        <li><a href="#section8">Results</a></li>
        <li><a href="#section9">Challenges and Limitations</a></li>
        <li><a href="#section10">Future Improvements</a></li>
        <li><a href="#section11">Conclusion</a></li>
        <li><a href="#section12">References</a></li>
    </ol>

  <h2 id="section1">1. Project Overview</h2>
    <p>The RFID-Based Door Access Control System is an embedded system that utilizes RFID (Radio-Frequency Identification) technology to control access to a secured area or a door. The system consists of an ESP8266 microcontroller, an RFID module, a 16x2 LCD display, and a web server. Users are required to authenticate using a web-based interface before being granted access.</p>

   <h2 id="section2">2. Objective</h2>
    <p>The main objective of this project is to create a secure and user-friendly access control system that provides controlled access to a specific area. The system should be able to:</p>
    <ul>
        <li>Allow authorized users to unlock the door using their RFID cards.</li>
        <li>Maintain a list of authorized users and their RFID card information.</li>
        <li>Allow administrators to add or remove users through a web interface.</li>
        <li>Provide a secure login mechanism for administrators to manage the system.</li>
    </ul>

   <h2 id="section3">3. Hardware Components</h2>
    <p>The following hardware components are used in the project:</p>
    <ul>
        <li>ESP8266 WiFi module</li>
        <li>MFRC522 RFID module</li>
        <li>16x2 I2C LCD display</li>
        <li>Electronic lock mechanism</li>
        <li>Buzzer</li>
        <li>LEDs</li>
        <li>Breadboard and connecting wires</li>
    </ul>

   <h2 id="section4">4. Software Components</h2>
    <p>The software components used in the project include:</p>
    <ul>
        <li>Arduino IDE for programming the ESP8266 microcontroller.</li>
        <li>Libraries such as Wire, MFRC522, LiquidCrystal_I2C, ESP8266WiFi, and ESP8266WebServer.</li>
        <li>Google Apps Script for cloud-based data storage.</li>
        <li>HTML and CSS for creating web interfaces.</li>
    </ul>

  <h2 id="section5">5. System Architecture</h2>
    <p>The system follows a client-server architecture:</p>
    <ul>
        <li>The ESP8266 microcontroller serves as the client and controls the hardware components.</li>
        <li>The Google Apps Script acts as a server to store and manage authorized user data.</li>
        <li>The web server running on the ESP8266 microcontroller provides a user interface for administrators and communicates with the Google Apps Script server.</li>
    </ul>

   <h2 id="section6">6. Functionalities</h2>
   <p>The RFID-Based Door Access Control System offers the following functionalities:</p>
    <ul>
        <li>RFID card authentication for access control.</li>
        <li>Web-based user interface for administrators to manage users.</li>
        <li>Real-time feedback through the 16x2 LCD display.</li>
        <li>Audible feedback using a buzzer.</li>
        <li>LED indicators for system status.</li>
        <li>Secure user authentication for administrators.</li>
        <li>Ability to add, remove, and view authorized users.</li>
    </ul>

  <h2 id="section7">7. User Guide</h2>
    <p><strong>For Administrators:</strong></p>
    <ol>
        <li>Connect to the system's WiFi network.</li>
        <li>Open a web browser and navigate to the system's IP address (default: http://&lt;ESP8266_IP&gt;/).</li>
        <li>Log in with the provided username and password.</li>
        <li>Add or remove users as needed.</li>
    </ol>
    <p><strong>For Users:</strong></p>
    <ol>
        <li>Present an authorized RFID card to the RFID module.</li>
        <li>The system will either grant or deny access and provide visual and audible feedback.</li>
    </ol>

   <h2 id="section8">8. Results</h2>
    <p>The RFID-Based Door Access Control System successfully provides access control based on RFID card authentication. Administrators can easily manage user access through a web interface, and the system provides real-time feedback to users.</p>

   <h2 id="section9">9. Challenges and Limitations</h2>
    <p><strong>Challenges and Limitations:</strong></p>
    <ul>
        <li>Limited storage capacity: The EEPROM storage of the ESP8266 has a limited capacity for storing user data.</li>
        <li>Security: While the system offers basic security for administrators, further security measures can be implemented.</li>
        <li>Scalability: The system may require additional features for scalability in larger environments.</li>
    </ul>

  <h2 id="section10">10. Future Improvements</h2>
    <p><strong>Future Improvements:</strong></p>
    <ul>
        <li>Implement a database for more extensive storage of user data.</li>
        <li>Enhance security features, such as multi-factor authentication.</li>
        <li>Enable remote access and control via a mobile app.</li>
        <li>Integrate with a cloud-based authentication service for user management.</li>
    </ul>

   <h2 id="section11">11. Conclusion</h2>
    <p>The RFID-Based Door Access Control System provides a secure and user-friendly solution for access control. It can be used in various applications, including homes, offices, and industrial facilities, to ensure authorized access to secured areas.</p>

  <h2 id="section12">12. References</h2>
    <p>References:</p>
    <ul>
        <li><a href="https://www.esp8266.com/">ESP8266 WiFi Module</a></li>
        <li><a href="https://github.com/miguelbalboa/rfid">MFRC522 RFID Module</a></li>
        <li><a href="https://www.arduino.cc/">Arduino IDE</a></li>
        <li><a href="https://www.google.com/script/start/">Google Apps Script</a></li>
        <li><a href="https://github.com/johnrickman/LiquidCrystal_I2C">LiquidCrystal_I2C Library</a></li>
        <li><a href="https://github.com/esp8266/Arduino">ESP8266WiFi Library</a></li>
        <li><a href="https://github.com/esp8266/Arduino">ESP8266WebServer Library</a></li>
    </ul>
</body>
</html>
