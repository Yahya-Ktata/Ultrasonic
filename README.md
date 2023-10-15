# Ultrasonic
Program uses a ATMega328p MCU to query a HC-SR04 ultrasonic module. Then Calculates and displays the distance to a object in cm on the LCD display.

![image](https://github.com/Yahya-Ktata/Ultrasonic/assets/144588719/8695e8c7-2539-4be1-83b0-49fd00670647)

This code is an implementation of an ultrasonic distance sensor using an AVR microcontroller. It initializes the LCD display and sets up timer interrupts, then enters an infinite loop where it sends out a pulse and measures the time it takes for the pulse to bounce back. The time is stored in two volatile variables and used to calculate the distance. The code also includes an interrupt service routine for the timer overflow interrupt.

The code uses several pins on the AVR microcontroller to interface with the ultrasonic distance sensor and the LCD display.
The PORTB pin is used to send out the pulse to the sensor. The DDRB pin is used to configure the PORTB pin as an output.
The TIMSK1 pin is used to enable the timer interrupts. The TIFR1 pin is used to clear the timer interrupt flag.
The ICR1 pin is used to read the timer capture value.
The LCD_RS, LCD_EN, LCD_D4, LCD_D5, LCD_D6, and LCD_D7 pins are used to interface with the LCD display. The LCD_RS pin is used to select the data to be displayed, the LCD_EN pin is used to enable the display, and the LCD_D4, LCD_D5, LCD_D6, and LCD_D7 pins are used to send the data to the display.
The mask variable is used to keep track of which pulse is being measured. The ov and ovf variables are used to keep track of the timer overflow and the previous timer capture value, respectively. The count variable is used to store the time it takes for the pulse to bounce back. The distance variable is used to store the calculated distance. The string variable is used to store the distance value as a string.

