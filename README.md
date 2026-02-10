FEMORA – Wearable Emergency Safety System
========================================

FEMORA is a wearable emergency safety system designed to provide instant assistance during critical situations using a single button press, without depending on smartphones or internet connectivity. The system combines RF communication, GPS tracking, and GSM-based alerts to ensure fast and reliable emergency response.

---

Project Overview
----------------

In emergency situations, accessing or operating a smartphone may not always be possible due to panic, low battery, or poor network conditions. FEMORA addresses this problem by providing a standalone, wearable safety solution that works independently of mobile applications and internet services.

The system consists of:
- A wearable transmitter unit (panic button device)
- A receiver/base unit (processing and communication module)

Once activated, FEMORA automatically retrieves the user’s real-time location and sends emergency alerts to predefined contacts.

---

System Architecture
-------------------

1. Transmitter Unit (Wearable Device)
- Worn on the wrist like a watch
- One-touch emergency activation
- Low power and lightweight

2. Receiver Unit (Base Station)
- Receives alert signals from the wearable
- Retrieves GPS location
- Sends SMS alerts and initiates phone calls using GSM

---

Working Principle
-----------------

1. User presses the emergency button on the wearable device  
2. Transmitter sends an RF alert signal  
3. Receiver unit detects the alert  
4. GPS module retrieves real-time latitude and longitude  
5. GSM module:
   - Sends an SMS with a Google Maps location link  
   - Makes an automatic emergency phone call  
6. Location updates can be sent periodically until the alert is stopped  

---

Hardware Components
-------------------

Wearable Transmitter Unit:
- Arduino Nano / Arduino Pro Mini  
- NRF24L01 RF Module  
- Push Button (Panic Button)  
- Rechargeable Battery  
- Power Switch  
- Watch-style Enclosure  

Receiver / Base Unit:
- Arduino Uno / Arduino Nano  
- NRF24L01 RF Receiver Module  
- GPS Module (Neo-6M)  
- GSM Module (SIM900A / SIM800)  
- SIM Card (for SMS and calls only)  
- 18650 Li-ion Batteries  
- Battery Holder  
- External Antenna  
- Project Enclosure  

---

Software and Technologies
-------------------------

- Embedded C / C++  
- Arduino IDE  
- RF24 Library  
- TinyGPS++ Library  
- GSM AT Commands  
- UART / Serial Communication  

---

Key Features
------------

- One-touch emergency alert  
- Wearable and portable design  
- No smartphone dependency  
- No internet requirement  
- Automatic SMS and call alerts  
- Live GPS location sharing  
- Reliable in low-network environments  

---

Applications
------------

- Personal safety systems  
- Women safety solutions  
- Child safety monitoring  
- Elderly emergency assistance  
- Wearable IoT safety devices  

---

Repository Structure
--------------------

FEMORA/
│
├── transmitter/
│ └── transmitter.ino
│
├── receiver/
│ └── receiver.ino
│
└── README.md


---

Setup and Usage
---------------

1. Upload the transmitter code to the wearable Arduino  
2. Upload the receiver code to the base unit Arduino  
3. Insert an active SIM card into the GSM module  
4. Power both units  
5. Press the emergency button to trigger alerts  

---

Future Enhancements
-------------------

- Auto-answer incoming calls from trusted contacts  
- Audio recording during emergencies  
- Geo-fencing alerts  
- Health monitoring sensors  
- Integration with emergency services  
- Miniaturized custom PCB  

---

Contributors
------------

1)Rajamurugan VS – Project Lead & Hardware Integration
 (Overall coordination, module integration, progress tracking)

2)Aravind Adityaa – System Workflow & Implementation Support
 (Understanding system flow, assisting development activities, coordination, basic validation)

3)Derrick Nathaniel D – GSM and Communication Modules
 (Handling GSM setup, message triggering, communication logic)

4)Krithik Ananth KA – RF Communication & Debugging
 (RF module configuration, signal testing, debugging support)

5)Arun Kumar – System Design & Documentation
 (System architecture, block diagrams, documentation)

6)Ram – Power Management & Battery Systems
 (Power supply planning, battery handling, power optimization)

---

License
-------

This project is licensed under the MIT License.  
See the LICENSE file for details.

---

Tagline
-------

One button. Instant help. No smartphone required.
