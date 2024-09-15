# UART Shell to control peripherals

## Revisions

| Date       | Student ID  | Student Name | Email                              | Project Link                                          |
| ---------- | ----------- | ------------ | ---------------------------------- | ----------------------------------------------------- |
| 15/09/2024 | 2024ht01143 | Pranav Ahuja | 2024ht01143@wilp.bits-pilani.ac.in | [Git Hub](https://github.com/pranav-ahuja/uart_shell) |

[toc]

## Scope

In this project the scope is to control the peripherals of the microcontroller using a UART shell. For the scope of thi project I have worked on controlling the LEDs on STM32F407 Microcontroller board. 

The user have to type commands on the serial monitor to control the peripherals.

## Requirements

### Hardware Requirement

- STM32F407VGT6

- FTDI converter (UART to TTL converter)

### Software Requirement

- STM32Cube IDE

- Tera Term Serial monitor

## Working

### STM32F407VGT6

The microcontroller STM32F407VGT6 is an ARM Cortex M4 based controller which is embedded on Discovery board. 
For the scope of this project we are using 2 peripherals:

1. UART - 
   
   - RX - PA3
   
   - TX - PA2

2. GPIO - 
   
   - Green LED - PD12
   
   - Red LED - PD14
   
   - Blue LED - PD15
   
   - Orange LED = PD13

### Commands

On the initial Window the menu is provided to the user asking for the option selected.

![](C:\Users\Pranav\AppData\Roaming\marktext\images\2024-09-15-15-23-44-image.png)

Upon selecting the option number(1,2,etc), the particular screen will be opened.

![](C:\Users\Pranav\AppData\Roaming\marktext\images\2024-09-15-15-24-49-image.png)

After this there are particular commands that are used to control the peripherals and then press enter.

| Commands           | Meaning                                  |
| ------------------ | ---------------------------------------- |
| turn on green led  | It is used to turn on the green leds     |
| turn on red led    | It is used to turn on the red leds       |
| turn on orange led | It is used to turn on the orange leds    |
| turn on blue led   | It is used to turn on the blue leds      |
| blink on led       | It is used to start blinking all the led |

### Turn on green LED

![](C:\Users\Pranav\AppData\Roaming\marktext\images\2024-09-15-15-33-07-image.png)


<img src="file:///C:/Users/Pranav/Desktop/green.jpg" title="" alt="" width="345">



### Turn on blue LED

![](C:\Users\Pranav\AppData\Roaming\marktext\images\2024-09-15-15-34-22-image.png)




<img src="file:///C:/Users/Pranav/Desktop/blue.jpg" title="" alt="" width="278">


### Turn on Orange LED

![](C:\Users\Pranav\AppData\Roaming\marktext\images\2024-09-15-15-35-12-image.png)


<img src="file:///C:/Users/Pranav/Desktop/orange.jpg" title="" alt="" width="286">



### Blinking the LED

![](C:\Users\Pranav\AppData\Roaming\marktext\images\2024-09-15-15-37-36-image.png)



<img src="file:///C:/Users/Pranav/Desktop/blink%20on.jpg" title="" alt="" width="326">


<img src="file:///C:/Users/Pranav/Desktop/blink_off.jpg" title="" alt="" width="332">



> By default the LED will blink at an interval of 1 second
