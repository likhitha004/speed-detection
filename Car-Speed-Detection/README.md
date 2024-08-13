# Car-Speed-Detection
This project is a simulation of a Car speed detector using IR sensors. This is simulated using Proteus Software

PRINCIPLE: 
IR Sensors are the main part of the project that detect the speed of a vehicle. Practically, you can implement the setup of IR Sensors in many ways but in this project, I have used two reflective type IR Sensors and placed them 5cm apart. 
When a vehicle travelling reaches the first sensor, the IR Sensor gets activated. From this moment onward, a timer is initiated and will continue to keep time until the vehicle reaches the second IR Sensor. 
By simulating the distance between the two sensors to be 5 centimetres, you can calculate the speed at which the vehicle travelled from IR Sensor 1 to IR Sensor 2 as you already know the time of travel. All the calculations and data gathering are done by Arduino and the final result is displayed on a 16X2 LCD Module.

CIRCUIT DESIGN:
The Digital OUT of the first IR Sensor is connected to Pin A0 of Arduino and the Digital OUT of the second IR Sensor is connected to Pin A1 of Arduino. Both the IR Sensors are provided with necessary power supply connections. The Digital OUT of the first IR Sensor is connected to Pin A0 of Arduino and the Digital OUT of the second IR Sensor is connected to Pin A1 of Arduino. Both the IR Sensors are provided with necessary power supply connections.
In order to view the vehicle speed details, I have used a 16×2 LCD. Its data pins i.e. D4 – D7 are connected to Digital I/O pins 7 -4. The RS and E pins of LCD are connected to pins 2 and 3 of Arduino. Rest of the connections are mentioned in the circuit diagram

WORKING:
The working of the Arduino based vehicle speed detector project is very simple. Arduino continuously reads the inputs from the IR Sensors. 
When a vehicle moving in front of the setup reaches the first sensor, Arduino becomes alert and capture a time stamp the moment the vehicle leaves the first IR Sensor. Another time stamp is recorded when the vehicle reaches the second IR Sensor. 
millis() function of Arduino used for capturing the time stamps. Arduino then calculates the velocity by assuming the distance as 5 centimetres between the two IR Sensors and displays the result in kilometres per hour on the 16×2 LCD Display




