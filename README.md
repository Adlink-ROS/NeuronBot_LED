# NeuronBot2_LED (Arduino Nano for example)

### Arduino IDE Installation

Search Arduino IDE on Ubuntu
<img src="https://github.com/Adlink-ROS/NeuronBot2_LED/blob/master/images/aduino_search.png">

Install Arduino IDE on Ubuntu Software
<img src="https://github.com/Adlink-ROS/NeuronBot2_LED/blob/master/images/arduino_install.png">

### Arduino IDE Setup and Sketch Upload

Click **Manage Libraries**
<img src="https://github.com/Adlink-ROS/NeuronBot2_LED/blob/master/images/arduino_manage_library.png">

Install **Adafruit NeoPixel** library for the Arduino Board.
<img src="https://github.com/Adlink-ROS/NeuronBot2_LED/blob/master/images/download_adafruit.png">

Set the **Board** to Arduino Nano
<img src="https://github.com/Adlink-ROS/NeuronBot2_LED/blob/master/images/Nano_BoardSet.png"> 

Set the **Processor** to ATmega328P (Old Bootloader)
<img src="https://github.com/Adlink-ROS/NeuronBot_LED/blob/master/images/processorset.png"> 

Find the actual path of symbolic link /dev/neuronbotLED in Ubuntu terminal
<img src="https://github.com/Adlink-ROS/NeuronBot_LED/blob/master/images/neuronbotLED.png"> 

Set the **Port** of Arduino IDE to /dev/ttyUSB*
<img src="https://github.com/Adlink-ROS/NeuronBot2_LED/blob/master/images/portset.png">

Open **Arduino_Nano.ino** in Arduino IDE
<img src="https://github.com/Adlink-ROS/NeuronBot2_LED/blob/master/images/arduino_open_sketch.png">

Click **Verify** button to verify the sketch

<img src="https://github.com/Adlink-ROS/NeuronBot2_LED/blob/master/images/verify.png">

Click **Upload** button to write the sketch into UNO

<img src="https://github.com/Adlink-ROS/NeuronBot_LED/blob/master/images/upload.png">

### Dependency installation on Ubuntu

Install the dependency
```sh
pip install pyserial   # if pip not found, use pip3 instead
```

### Check the function

Execute the script
```sh
python led_control.py --port /dev/neuronbotLED --mode 6
# port : the port where the USB cable is, e.g., /dev/neuronbotLED.
# mode : test built-in LED mode in this script
```
