Health Monitoring System using ESP32, MPU6050, MAX30100, and ThingSpeak
This project uses an ESP32 microcontroller in conjunction with various sensors to monitor health parameters like heart rate, SpO2 levels, pulse, and sweat levels. The data is then sent to ThingSpeak for remote monitoring and analysis.

Components Used
ESP32: The microcontroller used for reading sensor data and sending it to the ThingSpeak platform.
MAX30100: Sensor used for measuring heart rate (BPM) and SpO2 (blood oxygen saturation) levels.
MPU6050: Sensor for measuring acceleration (x, y, z) and gyroscopic data.
MCP3008: ADC used to read analog signals for pulse and sweat level.
ThingSpeak: Cloud platform for data logging and visualization.
Features
Real-time monitoring of:
Heart Rate (BPM)
Blood Oxygen Level (SpO2)
Pulse
Sweat Level
Acceleration (X-axis)
Data is uploaded to ThingSpeak for easy monitoring and analysis.
Pulse and SpO2 values are monitored, and data is only sent when certain thresholds are met (e.g., BPM > 50, SpO2 > 90).
Setup Instructions
Connect the following sensors to the ESP32:

MAX30100: For measuring heart rate and SpO2.
MPU6050: For acceleration and gyroscope data.
MCP3008: For pulse and sweat level measurements.
In the code, replace 688293 and 3C5X699IVKYNLOU7 with your own ThingSpeak Channel ID and API Key.

Upload the code to your ESP32 board.

Monitor the serial output to view real-time heart rate, SpO2, and sensor data.

Dependencies
Adafruit MAX30100: For heart rate and SpO2 measurements.
Adafruit MPU6050: For accelerometer and gyroscope readings.
ThingSpeak Library: For communication with the ThingSpeak platform.
Adafruit MCP3008: For ADC readings of pulse and sweat levels.
Install these libraries via the Arduino Library Manager.

Data Visualization
The data is uploaded to ThingSpeak where you can visualize the health parameters over time using ThingSpeak's charts and data analytics tools.

Future Enhancements
Add more sensors for additional health monitoring.
Implement real-time alerts when health parameters exceed certain thresholds.
