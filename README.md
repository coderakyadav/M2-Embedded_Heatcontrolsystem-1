[README.md](https://github.com/Mamtavishe/M2-Embedded_Heatcontrolsystem/files/7632241/README.md)
## M2-Embedded_Heatcontrolsystem

A heat control system is build using Atmega328.The button sensor first senses is a passenger or driver is onboarded in the car. When both button sensor and heat sensor are turned on the led glows.Only then the temperature sensor works and takes values from the ADC whose output is shown as pulse width modulation. All the data is transffered using UART communication protocal.

|**Folder**|**Description**|
| :- | :- |
|1_Requirements![image](https://user-images.githubusercontent.com/94283305/144180706-1628b82b-cc2e-4aca-8f84-b4083cc389d0.png)| Documents detailing requirements and research![image](https://user-images.githubusercontent.com/94283305/144180890-f1aa3c90-0420-4349-8a47-e11cb4514bbf.png)
|2_Architectures|Documents specifying design details|
|3_Implementation|All code and documentation|
|4_TestPlanandOutput|Outputs and Results after simulation|
|5_Simulation|SimulIDE Simaulation FIle|
|6_Images and Videos|Images, GIFS related to Outputs|

## Heat Control System 

### Theory

The heat control system is basically used to control the temperature of a car seat. When a user or driver of the car gets seated on a car, the button sensor gets activated. After that, the user gets access to turn on the heater. The temperature sensor keeps monitoring the temperature and sends the analog value to the microcontroller. The microcontroller processes the analog input of the temperature sensor and outputs a temperature value through serial communication. All the activities of the control system are done on a microcontroller called Atmega328.

### Simulation

The functionality of the heat control system is coded in embedded c and the working is demonstrated using simuation in a software called SimulIDE.
Below shows two images where in the 1st image shows the status of the simulation when the system is OFF and the second image shows the status of the system when it is ON. 

#### ON
![ON](https://github.com/hemanthasapu/embedded_systems_project_256889/blob/main/simulation/Simulation.gif)

#### OFF
![OFF](![Screenshot (335)](https://user-images.githubusercontent.com/94376599/144197395-ac7d91f3-5100-49b0-9b4c-805ca6bde339.png))

#### Outputs

|Circuit|RAM Table|
|:--:|:--:|
|![CIRCUIT](https://github.com/hemanthasapu/embedded_systems_project_256889/blob/main/simulation/Circuit.gif)|![RAM_TABLE](https://github.com/hemanthasapu/embedded_systems_project_256889/blob/main/simulation/RAM_table.gif)|
|CRO|Serial Monitor|
|![CRO](https://github.com/hemanthasapu/embedded_systems_project_256889/blob/main/simulation/Oscilloscope.gif)|![ON](https://github.com/hemanthasapu/embedded_systems_project_256889/blob/main/simulation/Serial_Monitor.gif)|

### Functionality 

* When the two switches are closed, the first LED glows indicating the actuation of the system and the heater.
* Next the analog input from the temperature sensor is received and digitized.
* The digitized temperature input is visualized using Pulse Width Modulation.
* The corresponding temperature values based on the digitized temperature input is transmitted by the UART protocol. Here the data is displayed on the serial monitor.





Codacy Badge

[![Codacy Badge](https://app.codacy.com/project/badge/Grade/78232789450b40daa10c0c74f810f497)](https://www.codacy.com/gh/Mamtavishe/M2-Embedded_Heatcontrolsystem/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=Mamtavishe/M2-Embedded_Heatcontrolsystem&amp;utm_campaign=Badge_Grade)

Code Quality Score

![Badge](https://api.codiga.io/project/30182/score/svg)

Code Grade

![BAdge](https://api.codiga.io/project/30182/status/svg)

Git Inspector

[![GitInspector](https://github.com/Mamtavishe/M2-Embedded_Heatcontrolsystem/actions/workflows/GitInspector.yml/badge.svg)](https://github.com/Mamtavishe/M2-Embedded_Heatcontrolsystem/actions/workflows/GitInspector.yml)

Cppcheck passing

[![C/C++ CI](https://github.com/Mamtavishe/M2-Embedded_Heatcontrolsystem/actions/workflows/c-cpp.yml/badge.svg)](https://github.com/Mamtavishe/M2-Embedded_Heatcontrolsystem/actions/workflows/c-cpp.yml)
[![CI](https://github.com/Mamtavishe/M2-Embedded_Heatcontrolsystem/actions/workflows/main.yml/badge.svg)](https://github.com/Mamtavishe/M2-Embedded_Heatcontrolsystem/actions/workflows/main.yml)

Linux Passing

[![Linux C/C++ CI](https://github.com/Mamtavishe/M2-Embedded_Heatcontrolsystem/actions/workflows/Linux-c-cpp.yml/badge.svg)](https://github.com/Mamtavishe/M2-Embedded_Heatcontrolsystem/actions/workflows/Linux-c-cpp.yml)
[![Compile-Linux](https://github.com/Mamtavishe/M2-Embedded_Heatcontrolsystem/actions/workflows/compile.yml/badge.svg)](https://github.com/Mamtavishe/M2-Embedded_Heatcontrolsystem/actions/workflows/compile.yml)
