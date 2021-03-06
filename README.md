# INTRODUCION
* The horizontal Lidar sensor in ANDBOT is located at 45cm off-the-ground.
* In in-door environment, there could be obstacles closed to the ground, which can not be detected by Lidar sensor.
* We put ultrasonic sensors to detect those obstacles.
* This document describes the ultrasonic hardware layout design. 

# ULTRASONIC SENSOR
* SENSOR SPEC (https://docs.google.com/document/d/1Y-yZnNhMYy7rwhAgyL_pfa39RsB-x2qR4vP8saG73rE/edit)
 * Power supply:+5V DC
 * Quiescent Current: <2mA
 * Working Currnt: 15mA
 * Effectual Angle: <15°
 * Ranging Distance : 2cm – 400 cm/1" - 13ft
 * Resolution : 0.3 cm
 * Measuring Angle: 30 degree
 * Trigger Input Pulse width: 10uS
 * Dimension: 45mm x 20mm x 15mm 
* In the manual, the effective FOV & ranging distance are not very clear. We searched forum discussions and we will take following parameters to design the coverage:
 * Horizon FOV: **22°**
 * Vertical FOV: **4°** 
 * Ranging Distance: **150cm**

# LAYOUT DESIGN
* Based on above parameters, the layout design and coverage is shown as below.

![](https://github.com/wennycooper/ANDBOT-ULTRASONIC-SENSORS-LAYOUT/blob/master/image.png)

* OBSTACLE RANGES
  * We will test the sensors in prototype and fine tune the **"obstacle_range"** & **"raytrace_range"** parameters in **costmap_common_params.yaml**
   * It should be 50cm+ 
