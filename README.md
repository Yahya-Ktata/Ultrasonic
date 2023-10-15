# Ultrasonic
Program uses a ATMega328p MCU to query a HC-SR04 ultrasonic module. Then Calculates and displays the distance to a object in cm on the LCD display.

![image](https://github.com/Yahya-Ktata/Ultrasonic/assets/144588719/8695e8c7-2539-4be1-83b0-49fd00670647)

This code is an implementation of an ultrasonic distance sensor using an AVR microcontroller. It initializes the LCD display and sets up timer interrupts, then enters an infinite loop where it sends out a pulse and measures the time it takes for the pulse to bounce back. The time is stored in two volatile variables and used to calculate the distance. The code also includes an interrupt service routine for the timer overflow interrupt.

