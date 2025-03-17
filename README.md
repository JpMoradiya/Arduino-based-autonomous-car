# Arduino-based-autonomous-car
Obstacle Detection &amp; Avoidance With Az-delivery Arduino Uno, L298N H-bridge, HC-SR04 Sensor (Ultrasonic Sensor), DC geared Motors


**Implementation of Hardware and Software**

1. First, we connected the DC motors to the L298N H-bridge: The L298N H-bridge is connected to the DC motors and is used to control their speed and direction. The Hbridge has two output pins and four input pins.
2. Attach the L298N H-bridge to the Az-delivery Arduino: The car's processing power and input/output interfaces come from the Az-delivery Arduino, which is connected to the L298N H-bridge. The digital pins of the Az-delivery Arduino are hooked up to the H-bridge.
3. Attach the HC-SR04 sensor to the Az-delivery Arduino: The distance measurements from the HC-SR04 sensor are read by the Az-delivery Arduino, which is connected to the sensor. The sensor is connected to two digital pins on the Az-delivery Arduino, one for the trigger signal and one for the echo signal.
4. In the next step, we set up the parameters for the sensor: The HCSR0.h library is used to set the parameters of the sensor, such as the maximum range, the length of the trigger pulse, and the time between measurements.
5. then Read the data from the sensor: The Az-delivery Arduino's microcontroller reads the data from the sensor by sending a trigger signal to the HC-SR04 sensor and timing how long it takes for the echo signal to return. Then, using the speed of sound and the time of flight, the distance is worked out.
6. Next, we Control the speed and direction of the motors. The microcontroller figures out the right speed and direction for the motors based on the data from the sensors and sends the appropriate signals to the L298N H-bridge. Changes in the voltage sent to the motors through the H-enable bridge's pins change the speed of the motors.
7. Run obstacle avoidance algorithms. Using the sensor data, the microcontroller runs obstacle avoidance algorithms to figure out where the car is going and how to avoid obstacles.
8. Next, we Write the code for the software: Programming the Az-delivery Arduino is done with the Arduino IDE, where the software code is written. The code is used to set up the parameters for the sensors, read the data from the sensors, control the speed and direction of the motors, and run the algorithms for avoiding obstacles.
9. then we Upload software code: The Arduino IDE and a USB cable are used to send the software code to an Az-delivery Arduino.
10. finally, Test the self-driving car: The self-driving car is tested in different environments to make sure it can find and avoid obstacles.

**Architecture of Self-Driven Car**
![Picture1](https://github.com/user-attachments/assets/6d759f67-a0e6-43b6-9ba8-a7ef4cb729ac)
