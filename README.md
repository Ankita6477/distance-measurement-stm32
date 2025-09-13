## Distance-measurement-stm32
This is an embedded systems project for interfacing an ultrasonic distance sensor (HC-SR04) with an STM32 microcontroller using STM32CubeIDE and the HAL libraries. The measured distance is displayed on a 16x2 LCD in real-time. This project is useful for learning how to use GPIO, timers, and peripheral interfacing on STM32 microcontrollers.

##📖 Description
This STM32-based embedded system project reads distance measurements from an HC-SR04 ultrasonic sensor and displays the results on a 16x2 I2C LCD using the HAL library and STM32CubeIDE.
The purpose is to demonstrate how to integrate sensors and displays with STM32 microcontrollers for real-time data visualization, useful in basic robotics, obstacle detection, and smart measurement applications.

##🔧 Features

📏 Measures distance using HC-SR04 ultrasonic sensor
📺 Displays distance (in cm) on I2C 16x2 LCD
🔁 Real-time continuous reading with 1-second interval
🧠 Uses STM32 HAL drivers (not bare-metal register programming)
🧰 Built with STM32CubeIDE

##⚙️ Hardware Used
Component	Description
STM32F103C8T6 ("Blue Pill")	Main microcontroller board
HC-SR04	Ultrasonic distance sensor
16x2 LCD + I2C Module	LCD for displaying output
Jumper Wires, Breadboard	For connections
5V USB Power	To power the STM32 board

##🔌 Connections
🟢 Ultrasonic Sensor:
HC-SR04 Pin	STM32 Pin
VCC    	5V
GND   	GND
TRIG  	PA9
ECHO	  PA8
🔵 I2C LCD:
I2C Pin	STM32 Pin
SDA	PB7 (I2C1 SDA)
SCL	PB6 (I2C1 SCL)

You can configure these pins via STM32CubeMX .ioc file.

##💻 Software Tool
STM32CubeIDE
STM32 HAL Drivers
Custom lcd.h/.c and ultrasonic.h/.c files for abstraction
