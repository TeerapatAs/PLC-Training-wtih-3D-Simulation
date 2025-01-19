# PLC-Training-with-3D-Simulation
Design and simulate PLCs in different scenarios. Case 1-4 is simulated in Mitsubishi FX-TRN-BEG-E, and Case 5 is in Codesys.
In case 5, the PLC program Cutting Machine was implemented in the PLC Modules Benchmark and satisfied the specifications.

![image](https://github.com/user-attachments/assets/8ba84b81-0fac-4eba-9df5-63e9359445db)

## 1. Operating Lamp
**Control Specifications**
1) When Switch 1 (X24) on the table is pressed, Green Lamp (Y0) is lit.
If Switch 1 (X0) is turned off, Green Lamp (Y0) remains lit.
2) When Switch 2 (X25) is pressed, Yellow Lamp (Y1) is lit.
If Switch 2 (X25) is turned off, Yellow Lamp (Y1) is off.
3) When Button 1 (X20) or Button 2 (X21) is pressed, Red Lamp for error (Y2) is lit.



https://github.com/user-attachments/assets/05ce23a8-458b-4e3f-a593-39eb52a7e0c6

## 2. Loop Operation with latched input
https://github.com/user-attachments/assets/e52b987f-8f7c-43a4-8315-65a50fdf97c4

## 3. Detecting Sensors with Differentiation Between Detection Cases
**Human side**
1) When the sensor In gate (X0) detects a person, the flashing light Green (Y1) comes ON.
2) 5 seconds after the sensor Out (X1) detects the passage of the person, the flashing light green (Y1) is extinguished.

https://github.com/user-attachments/assets/804e8f77-6085-4c26-841e-33845396282f


**Car side**
1) When the sensor In gate (X2) detects a car, the flashing light Green (Y4) is lit.
2) 5 seconds after the sensor Out (X3) detects the passage of the car, the flashing light Green
(Y4) is extinguished.
3) If the car does not pass through the area between In gate (X2) and Out (X3) within 10
seconds, the flashing light Red (Y3) is lit, and Buzzer (Y7) sounds.
4) As soon as the car has passed the sensor Out (X3), the flashing light Red (Y3) is
extinguished and Buzzer (Y7) stops.

https://github.com/user-attachments/assets/040d547a-205b-4d2f-9c80-01c9d53ac672

## 4. Traffic Light Sequence
1) When [PB1] (X20) on the operation panel is pressed, the process is started.
2) First, the signal lamp Red (Y0) is lit for 10 seconds.
3) The signal lamp Red (Y0) is extinguished after it has been lit for 10 seconds. The signal lamp
Yellow (Y1) is lit for 5 seconds.
4) The signal lamp Yellow (Y1) is extinguished after it has been lit for 5 seconds. The signal
lamp Green (Y2) is lit for 10 seconds.
5) The signal lamp Green (Y2) is extinguished after it has been lit for 10 seconds.
6) The operations starting from 2) above are repeated.

https://github.com/user-attachments/assets/533cac08-4ecc-42fd-a6f4-7c4e5ac50483

## 5. Cutting Machine
![Cutting Machine Instructions](https://github.com/user-attachments/assets/27671acb-b7b0-40ad-b27b-e84dce3346ea)

https://github.com/user-attachments/assets/a96bdb17-369d-4d6a-ac31-7faf97b25d70



