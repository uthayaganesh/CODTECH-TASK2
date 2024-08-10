# CODTECH-Task-2

NAME:UTHAYA GANESH M

COMPANY: CODTECH IT SOLUTIONS

ID: CTO8DS5O56

DOMAIN: IOT

DURATION: JULY 15-AUGUST 15 2024

MENTOR: MUZAMMIL AHMED

Project: Weather Monitoring Station

Objective

Create an IoT-based system to collect and display real-time data on temperature, humidity, and atmospheric pressure via a mobile app.

Key Activities

Integrate temperature, humidity, and pressure sensors with an ESP8266/ESP32 microcontroller. Develop firmware to send sensor data to a Firebase cloud database. Build a mobile app using MIT App Inventor to display the data in real-time. Test the system for accuracy and reliability, deploy the hardware, and maintain the system with regular updates and support.

Technologies Used

Sensors (DHT22, BMP280), microcontroller (ESP8266/ESP32), Firebase for cloud storage, MIT App Inventor for the mobile app, and Wi-Fi for data transmission.

Key Insights

Ensure accurate sensor data collection and secure data transmission. Provide real-time data on an intuitive mobile app. Regularly update and maintain the system for consistent performance and user satisfaction.


Create a Mobile App Using MIT App Inventor
1. Start a New Project:
* Open MIT App Inventor and create a new project.
2. Design the User Interface:
* Drag and drop three Label components onto the screen. These will be used to display temperature, humidity, and pressure.
* Add a FirebaseDB component to connect the app to your Firebase database.
* Include a Clock component to periodically fetch data from Firebase.
3. Configure FirebaseDB Component:
* Set the FirebaseURL property to https://YOUR_FIREBASE_PROJECT_ID.firebaseio.com/.
* Set the FirebaseToken property to your Firebase database secret.
4. Set Up the Blocks Editor:
* Initialize Labels:
o Set the initial text for each label to "Loading...".
* Clock Timer:
o Configure the Clock component to periodically call the FirebaseDB.GetValue method for each data point (temperature, humidity, pressure).
* Handle Firebase Data:
o In the FirebaseDB.GotValue event, check the Tag to identify which data (temperature, humidity, or pressure) was retrieved.
o Update the corresponding label with the retrieved value.
