# Max8: Adafruit AMG8833 Thermal Camera Heatmap Jitter

This repository contains the Max/MSP/Jitter code, for visualising data from the Adafruit thermal camera. The camera is a heatcamera with an 8 x 8 pixel dimension, that can measure temperatures between 0 to 80 degrees celsius. the sensor is capable of registering a human of up to 7 meters away, acording to Adafruit.

<img src="./media/Adafruit AMG8833 Thermal camera Max-patch Jitter.png" alt="Schematic" style="zoom: 100%;" />

## Adafruit AMG8833 Setup

In order to use the max-patch, you must first start by following adafruits guide, in order to setup the camera with an arduino. This involves constructing the circuit below.

<img src="./media/Adafruit AMG8833 connected to Arduino.png" alt="Schematic" style="zoom: 100%;" />

And downloading the "Adafruit_AMG88xx library", by following this path

![](https://cdn-learn.adafruit.com/assets/assets/000/048/539/large1024/temperature___humidity_managelib.png?1511746137)

Type in **AMG88xx** until you see the Adafruit Library pop up. Click Install!

![](https://cdn-learn.adafruit.com/assets/assets/000/048/540/large1024/temperature___humidity_amglib.png?1511746208)

the final step of setting up the Adafruit AMG8833 is to check if it is working by running the "amg88xx_test" example code, and checking to see that the serial monitor outputs (room temperature). If all here looks good, you are done with the setup.

**File->Examples->Adafruit_AMG88xx->amg88xx_test**

![](https://cdn-learn.adafruit.com/assets/assets/000/043/121/large1024/temperature_serialtest.gif?1498596216)

## Getting Started

Once it is setup then upload the example called "pixel_test" to the arduino.

**File -> Examples -> Adafruit_AMG88 -> pixels_test**

when you have uploaded the code **it is important that you do NOT open the serial monitor in the arduino IDE.** Instead you open the Max-patch and press the toggle button in order to initiate the patch.

then you select the corresponding serial port from the drop down menu, and now the code should be running as intended.

(optional) you can fullscreen the visualizer by pressing ESC, and exit fullscreen by once again pressing ESC.


## Sources:
- https://github.com/DDlabAU/thermal-camera-heatmap
- https://cdn-learn.adafruit.com/downloads/pdf/adafruit-amg8833-8x8-thermal-camera-sensor.pdf
- http://www.electroschematics.com/wp-content/uploads/2013/01/Arduino-Uno-R3-Pinouts.png