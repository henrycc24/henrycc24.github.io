+++
title = "Lab 1"
description = "Connecting Bluetooth to the Nano"
date  = 2025-01-31
+++

> Lab1: The Artemis Board and BlueTooth


## Prelab
Before starting the lab we had to setup our computers in order for us to work with the Adruino. Doing this requrired us downloading the **Arduino IDE**. Luckily for me even though I have a Mac, I haven't updated it in years, so I don't have to download any additional drivers. Getting that out of the way, next I had to setup my environemnt in Python in order to send and recieve messages from the ardruino, Having Pip and Python latest versions already installed all I had to do was download the virtual environment (activate it), downlaod the necessary python packages, the codebase, and Jupyter Notebook. 



```python
source FastRobots_ble/bin/activate
pip install numpy pyyaml colorama nest_asyncio leak jupyterlab
```

The codebase we are working in is ble_arduino where it has the files ble_arduino.ino, BLECstringCharacteristic.h, EString.h, RobotCommand.h which to sum up do: 

**RobotCommand.h**
 - Used when Artemes recieves string format of 
```python
<cmd_type>:<value1>|<value2>...
```
- robot_cmd(:|) whrere ":l" is deilmiter 
- <cmd_type> is an int and <value> can be either an int, float, string 
- Main way we will by sending commands in jupyter notebook

**EString.h.h**
- Used to manipulate char arrays
- provides getter and setter functions 
- Clear(), append(), c_str(), are all used throuhgout to send charracter arrays. 
- Used to transmit strings from the Artemis to the computer (main way we recieve data in lab)

**BLECstringCharacteristic.h**
- Use to receive data from the artemis 
- writeValue(value): the value is what we transmit to the computer 

**ble_arduino.ino**
- Main file we will be editing and connecting though our Artemis wth BLE 
- Contains our UUIDS (University unique identifiers) 

Furthermore, we had to configure ble_arduino such that we print the MAC_ADDRESS and create a new UUID

## The Process

We follow below simple steps to build websites and applications,

- You contact us with a requirement of static, dynamic website or web application.
- We analyze the requirements and come up with a proposal of estimate time and cost involved.
- We send you some example themes from which you can choose.
- After you complete advance payment, we start development.
- We will keep you updated with the progress in stages with demo of the website.
- After the final demo and your final payment, the website will be live.


**Please note that you can contact us even if you are not sure whether a web application is suitable for your process or not.**