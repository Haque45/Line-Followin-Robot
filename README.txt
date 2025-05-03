🚗 PID Line Following Robot
This project implements a PID (Proportional-Integral-Derivative) controlled Line Following Robot using 5 infrared sensors for line detection and 4 motor control pins for direction and speed regulation.

🛠️ Features
Real-time sensor-based line tracking using 5 digital IR sensors.

PID control for smooth and accurate navigation.

Adjustable PID constants (Kp, Ki, Kd) for fine-tuning performance.

🧰 Hardware Requirements
Arduino board (e.g., Uno, Mega, etc.)

5 IR line sensors

Motor driver (L298N or similar)

2 DC motors (differential drive)

Power supply

Chassis

🧾 Pin Configuration
Function	Pin No
Sensor 1	D25
Sensor 2	D32
Sensor 3	D33
Sensor 4	D26
Sensor 5	D35
Left Motor IN1	D13
Left Motor IN2	D12
Right Motor IN3	D27
Right Motor IN4	D14

📦 Code Overview
Sensor Reading: Reads digital values from 5 sensors to detect line position.

Error Calculation: Assigns weights to sensor input and computes positional error.

PID Control: Uses error, integral, and derivative terms to calculate motor speed correction.

Motor Control: Adjusts motor speed to keep the robot on track.

🔧 PID Tuning Parameters
cpp
Copy
Edit
float Kp = 25;
float Ki = 0;
float Kd = 15;
Adjust these constants to optimize performance on different tracks.

🧪 Getting Started
Wire up sensors and motors as described.

Upload the sketch to your Arduino board.

Place the robot on a contrasting line path and power it up.

Fine-tune PID constants for better accuracy.

📜 License
This project is open-source and available under the MIT License.

