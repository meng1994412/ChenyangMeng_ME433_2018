# Advanced Mechatronics in Mechatronics Systems Prototyping
## Project Obejctives
* Design, solder, and debug a printed circuit board (PCB).
* Implement advanced digital communication protocals like SPI, I2C, USB, CAN.
* Design the prototype with SolidWorks.
* Create physical prototypes with a laser cutter, and a 3D printer.
* Interface with Android device.

## Software/Language Used
* C
* [MPLAB X IDE v4.15](http://www.microchip.com/mplab/mplab-x-ide)
* [MPLAB XC32/32++ Compiler v1.44](http://www.microchip.com/mplab/compilers)
* [MPLAB Harmony Integrated Software Framework v2.05.01](http://www.microchip.com/mplab/mplab-harmony)
* [EAGLE PCB](https://www.autodesk.com/products/eagle/free-download)
* [Android Studio](https://developer.android.com/studio/)
* [SolidWorks](https://www.solidworks.com/)

## Hardware Used
* [Microchip(PIC32MX250F128B)](http://www.microchip.com/wwwproducts/en/PIC32MX250F128B)
* [Microchip(PICkit3)](http://www.microchip.com/Developmenttools/ProductDetails.aspx?PartNO=PG164130)
* [PCB](https://github.com/meng1994412/ChenyangMeng_ME433_2018/blob/master/HW3/picture%20of%20board.PNG)
* [Microchip(MCP4902)](https://github.com/meng1994412/ChenyangMeng_ME433_2018/blob/master/HW4/MCP4912DataSheet.pdf)
* [Microchip(MCP23008)](https://github.com/meng1994412/ChenyangMeng_ME433_2018/blob/master/HW5/i2cDataSheet.pdf)
* [TFT LCD](https://www.aliexpress.com/item/Free-Shipping-1-8-inch-TFT-touch-LCD-Module-LCD-Screen-Module-SPI-serial-51-drivers/32263827143.html)
* [IMU(LSM6DS33)](https://www.pololu.com/product/2736)

## Weekly Milstones
### Week 1
* Build and program a PIC32MX250F128B circuit board. ([details here](https://github.com/meng1994412/ChenyangMeng_ME433_2018/tree/master/HW1))

Here is the circuit board:

<img src="https://github.com/meng1994412/ChenyangMeng_ME433_2018/blob/master/HW1/Results/6_Breadboard.JPG" width="400">

### Week 2
* Design a PIC32MX250F128B library and schematic on EAGLE. ([details here](https://github.com/meng1994412/ChenyangMeng_ME433_2018/tree/master/HW2))
* Build a PIC32MX250F128B PCB on EAGLE. ([details here](https://github.com/meng1994412/ChenyangMeng_ME433_2018/tree/master/HW3))

Here is the schematic:

<img src="https://github.com/meng1994412/ChenyangMeng_ME433_2018/blob/master/HW2/picture%20of%20schematic.PNG" width="800">

Here is the PCB:

<img src="https://github.com/meng1994412/ChenyangMeng_ME433_2018/blob/master/HW3/picture%20of%20board.PNG" width="500">

### Week 3
* Build the MCP4912 DAC circuit and write a library to communicate with it via SPI. ([details here](https://github.com/meng1994412/ChenyangMeng_ME433_2018/tree/master/HW4))
* Build the MCP23008 I/O expander circuit and write a library to communicate with it via I2C. ([details here](https://github.com/meng1994412/ChenyangMeng_ME433_2018/tree/master/HW5))

Here is sine wave and triangle wave generated by SPI communication between MCP4912 and PIC32:

<img src="https://github.com/meng1994412/ChenyangMeng_ME433_2018/blob/master/HW4/Results/nScope%20reading.png" width="700">

Here is demo of communication between MCP23008 and PIC32:

![demo1](https://github.com/meng1994412/ChenyangMeng_ME433_2018/blob/master/HW5/Results/hw5demo.gif)

### Week 4
* Build communication between PIC32MX250F128B and TFT LCD via SPI. ([details here](https://github.com/meng1994412/ChenyangMeng_ME433_2018/tree/master/HW6))
* Solder IMU breakout board onto heahders pins. ([Picture](https://github.com/meng1994412/ChenyangMeng_ME433_2018/blob/master/HW7/CircuiteDiagram.JPG))
* Build communication between PIC32MX250F128B and IMU via I2C. ([details here](https://github.com/meng1994412/ChenyangMeng_ME433_2018/tree/master/HW7))

Here is a demo of LCD display:

![demo1](https://github.com/meng1994412/ChenyangMeng_ME433_2018/blob/master/HW6/Results/hw6demo.gif)

Here is a demo of IMU reading on LCD screen:
![demo1](https://github.com/meng1994412/ChenyangMeng_ME433_2018/blob/master/HW7/Results/hw7demo.gif)

### Week 5
* Rebuild communication between PIC32MX250F128B and IMU via I2C by using Harmony framework. ([details here](https://github.com/meng1994412/ChenyangMeng_ME433_2018/tree/master/HW8))
* Build communication between PIC32MX250F128B (including IMU, LCD) and computer ([PuTTY](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html)) via USB (communication class device (CDC)) by using Harmony framework so that PuTTY can obtain data value from IMU. ([details here](https://github.com/meng1994412/ChenyangMeng_ME433_2018/tree/master/HW9))

Here is a demo of communication between PIC32 and PuTTY:

![demo1](https://github.com/meng1994412/ChenyangMeng_ME433_2018/blob/master/HW9/Results/hw9demo.gif)

### Week 6
* Add digital signal processing (DSP) filter, including moving average filter (MAF), finite impulse response filter (FIR), and infinite impulse response filter (IIR), on z accleration of IMU to get rid of high frequency noises. ([details here](https://github.com/meng1994412/ChenyangMeng_ME433_2018/tree/master/HW10))
* Build communication between PIC32MX250F128B (including IMU, LCD) and computer via USB (human interface device (HID)) by using Harmony framework so that IMU can control the mouse on PC. ([details here](https://github.com/meng1994412/ChenyangMeng_ME433_2018/tree/master/HW11))

Here is a plot of raw data, and filtered data:

<img src="https://github.com/meng1994412/ChenyangMeng_ME433_2018/blob/master/HW10/Results/filter_plot2.png" width="500">

more details about the filter: [check here](https://github.com/meng1994412/ChenyangMeng_ME433_2018/blob/master/HW10/README.md)

Here is a demo for IMU controlling the mouse on PC via USB communication (HID):

![demo1](https://github.com/meng1994412/ChenyangMeng_ME433_2018/blob/master/HW11/Results/hw11demo.gif)

### Week 7
* Write a simple app (named HelloWorld) for a Android device ([Moto G](https://www.amazon.com/gp/product/B00HPP3VW2/ref=s9_acsd_hps_bw_c_x_4_w) version 4.4.4), which have a slide that displays a value from 0 to 100, and buttons to increase, decrease, and reset the slide bar value. ([details here](https://github.com/meng1994412/ChenyangMeng_ME433_2018/tree/master/HW12))
* Write a camera app (named ColorDetector)for Android device e ([Moto G](https://www.amazon.com/gp/product/B00HPP3VW2/ref=s9_acsd_hps_bw_c_x_4_w) version 4.4.4)that when pointing the camera at a green object, the app should identify the green shape and draw lines on top of it. ([details here](https://github.com/meng1994412/ChenyangMeng_ME433_2018/tree/master/HW13))

Here is a demo of how HelloWorld app works:

![demo1](https://github.com/meng1994412/ChenyangMeng_ME433_2018/blob/master/HW12/Results/hw12demo.gif)

Here is a demo for how ColorDetector app works (with adjustable sensitivity) on a RAZER mouse box:

![demo1](https://github.com/meng1994412/ChenyangMeng_ME433_2018/blob/master/HW13/Result/demo.gif)

### Week 8
* Solder the PCB with components from breadboard. ([details here](https://github.com/meng1994412/ChenyangMeng_ME433_2018/tree/master/HW14))
* Build a USB communication (class CDC) between PIC32 PCB and Android phone by writing a PIC32 program and Android app (named My Application), which PIC32 program will send a number to Android phone 5 times per second, and Android app has a slider to update value, a button to press to send the value of the slider to the PIC, a textview to show what was sent to the PIC, and a textview wrapped in a scrollview to show what was received from the PIC. ([details here](https://github.com/meng1994412/ChenyangMeng_ME433_2018/tree/master/HW14))

Here is the picture for PCB after soldering with components:

<img src="https://github.com/meng1994412/ChenyangMeng_ME433_2018/blob/master/HW14/Results/PCBsoldering.JPG" width="500">

Here is the screen of Android app:

<img src="https://github.com/meng1994412/ChenyangMeng_ME433_2018/blob/master/HW14/Results/AndroidScreen.png" width="500">

Here is the demo of how communication beteen PIC32 and Android device work:

![demo1](https://github.com/meng1994412/ChenyangMeng_ME433_2018/blob/master/HW14/Results/hw14demo.gif)

### Week 9
* Designed the wheel part and robot box parts by using [SolidWorks](https://www.solidworks.com/). ([details here](https://github.com/meng1994412/ChenyangMeng_ME433_2018/tree/master/HW15))

Here is a picture of wheel design:

<img src="https://github.com/meng1994412/ChenyangMeng_ME433_2018/blob/master/HW15/Wheel/Wheel.PNG" width="400">

Here is a picture of box assembly design:

<img src="https://github.com/meng1994412/ChenyangMeng_ME433_2018/blob/master/HW15/Box/Box.PNG" width="600">

### Week 10
* Make PI controller for wheel velocity and steering. ([details here](https://github.com/meng1994412/ChenyangMeng_ME433_2018/tree/master/HW16))
* Build an image processing app on Android device so that the robot is able to detect the road on the [map](https://github.com/meng1994412/ChenyangMeng_ME433_2018/blob/master/HW17/Results/techCup2018.png). ([details here](https://github.com/meng1994412/ChenyangMeng_ME433_2018/tree/master/HW17)).

* Utilize 3D printer to produce the wheels of the robot.
* Utilize laser cutting machine to produce the robot box.
* Assemble the all the parts together.
* Combine the image processing on Android device and PI controller on PIC32 together.
* For final project check [details here](https://github.com/meng1994412/ChenyangMeng_ME433_2018/tree/master/HW18).

Here is a picture of the robot:

<img src="https://github.com/meng1994412/ChenyangMeng_ME433_2018/blob/master/HW18/Results/robot.JPG" width="600">

Here is a demo for the robot following map:

![demo](https://github.com/meng1994412/ChenyangMeng_ME433_2018/blob/master/HW18/Results/demo.gif)
