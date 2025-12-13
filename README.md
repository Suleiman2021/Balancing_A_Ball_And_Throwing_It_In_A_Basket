## **Ball Balancing and Throwing System**

This project demonstrates an intelligent mechanism capable of balancing a ball at the center of a movable rudder, then launching it into a target basket using a controlled servo-based ejector system.

---

## **📌 Overview**

The system uses a servo motor connected to the rudder via a metal wire to control the ball’s lateral movement.
The ball shifts left when the servo angle is around **130°**, and right when it reaches **0°**.
The ball oscillates until it stabilizes at the center.

An **ultrasonic sensor** continuously measures the ball’s position. A **PID controller** adjusts the servo angle to maintain the ball at the reference point — the center of the rudder.

After achieving stable balance, the system moves the ball toward the ejector, where a second mechanism launches it into a target basket.

---

## **⚙️ How It Works**

### **1. Ball Balancing Module**

* A servo motor tilts the rudder left and right.
* The ball’s position is measured using an ultrasonic sensor.
* A PID controller:

  * Takes the distance measurement.
  * Compares it with the target center point.
  * Adjusts the servo angle accordingly until the ball is perfectly balanced.

### **2. Ball Transfer**

* Once balanced, the servo moves the ball toward the far-left edge (servo ~180°).

### **3. Ball Throwing Mechanism**

The launcher consists of:

* A structural frame.
* Two servo motors:

  * **Servo 1:** Controls the basket arm (usually positioned at 180°).
  * **Servo 2:** Pulls a rubber band used to launch the ball.

A distance sensor checks whether the basket is correctly aligned.

The system then:

1. Tightens the rubber band.
2. Releases the ejector arm by repositioning the servo.
3. Launches the ball toward the goal basket.

---

## **🧩 Components Used**

* Servo motor(s)
* Ultrasonic distance sensor
* PID controller (software implementation)
* Mechanical rudder
* Ball ejector with rubber band mechanism
* Structural frame / chassis
* Microcontroller (Arduino, ESP, etc.)

---

## **🚀 Features**

* Automatic ball balancing using PID
* Dynamic servo control based on sensor feedback
* Automated ball launching system
* Dual-module system (balancing + throwing)
* Real-time distance measurement

---


## **📸 Media**

[Balancing_A_Ball_And_Throwing_It_In_A_Basket.pdf](https://github.com/user-attachments/files/24103175/Balancing_A_Ball_And_Throwing_It_In_A_Basket.pdf)


https://github.com/user-attachments/assets/533fc637-8650-48ab-b15e-a0d3cc8db162

