# Smart Irrigation System - Final Project
Developed by: Dor Alagem

This is my final project for the IoT course. I built this system to show how we can monitor soil moisture and control irrigation remotely using the MQTT protocol.

## How it works
The system consists of a sensor (the Node) that sends data to a central controller (the Manager). If the soil gets too dry, the system alerts the user. I also added a web dashboard to see the history of the moisture levels.

## Tools I Used
* **Python** for the main logic.
* **MQTT** for sending messages between parts.
* **SQLite** to save the data.
* **Streamlit** for the web dashboard.
* **PyQt5** to create the sensor emulator window.
* **Icecream & Logging** to keep track of what's happening in the code.

## The Files in this Project
* `mqtt_init.py`: All the connection settings and topics.
* `app_manager.py`: The "brain" that saves data and checks if it's too dry.
* `irrigation_node.py`: The emulator with the button and the moisture sensor.
* `main_dashboard.py`: The website where you can see the graphs.

## How to run it
1. Install the requirements: `pip install paho-mqtt streamlit pyqt5 icecream pandas`
2. Run `app_manager.py` first.
3. Run `irrigation_node.py` to start the sensor.
4. Run `streamlit run main_dashboard.py` to see the dashboard.
