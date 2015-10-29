# INTRODUCION
* The horizontal Lidar sensor in ANDBOT is located at 45cm off-the-ground.
* In in-door environment, there could be obstacles closed to the ground, which can not be detected by Lidar sensor.
* We put ultrasonic sensors to detect those obstacles.
* This document describes the ultrasonic hardware layout design. 

# ULTRASONIC SENSOR
* SENSOR SPEC
 * Power supply:+5V DC
 * Quiescent Current: <2mA
 * Working Currnt: 15mA
 * Effectual Angle: <15°
 * Ranging Distance : 2cm – 400 cm/1" - 13ft
 * Resolution : 0.3 cm
 * Measuring Angle: 30 degree
 * Trigger Input Pulse width: 10uS
 * Dimension: 45mm x 20mm x 15mm 
* In the manual, the effective angle value & ranging distance is not very clear. We searched forum discussions and we will take parameters of the sensor as following:
 * Measurement angle: **22 degree**
 * Ranging Distance: **150cm**

Based on those parameters, the layout and coverage is shown as below.

![](https://github.com/wennycooper/ANDBOT-ULTRASONIC-SENSORS-LAYOUT/blob/master/image.png)
# 
