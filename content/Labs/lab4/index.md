+++
title = "Lab 4"
description = "Fourth Lab - Motor Control"
date  = 2025-01-31
+++

> Lab1: Motor and Open Loop Control 


## Prelab
Before starting the lab we must refreshen up on how to use the oscilloscope and check out the documenation/datasheet for the dual motor driver. While also carefully considering how we would like to arrange our sensors in our car. Note that we use seperate batteries for the motors/artemis since the motors consume more power then the artemis. As well as that the artemis won't be affected by any noise by the motors. 

![alt text](Circuit_dia.PNG)

# Tasks

# Lab 4

## **1. PWM Signals**

[![](https://markdown-videos-api.jorgenkh.no/youtube/p49Bavg1Acw)](https://youtu.be/p49Bavg1Acw)

After soldering the motor controllers, befeore I attach them to the motors I tested them out first using an oscilliscope and power supply. To mimic what we will be using as power, I set the power-supply to 3.7 volts. Hooking up the Vin and GND to the power supply, and then Bout1/Aout1 to GND and Bout2 and Aout2 to prope we get these images: 

![alt text](Oscill.PNG)  ![alt text](Osee_dia.PNG)

Running These Code: 

![alt text](OsCode.PNG)

## **2. Take it APART!**

Now we must create an empty husk of the former car shown below: 

![alt text](car_empty.PNG)



## **3. Spinning Motors**



Now we test if our motors function properly. I tested both motors at the same time with a power supply then only with a battery using 150 PWM on both. I tested it going forward and then going backwards as shown: 

Power Supply: 

[![](https://markdown-videos-api.jorgenkh.no/youtube/NanhYhcpWdQ)](https://youtu.be/NanhYhcpWdQ)

Battery:

[![](https://markdown-videos-api.jorgenkh.no/youtube/4oOiWewazSU)](https://youtu.be/4oOiWewazSU)

Code Used: 

![alt text](Test_motors.PNG)


## **4. Stuff It IN!**

Now we must stuff all the sensors we've been working on the previous labs inside the car. Now to make sure there wasn't to much wire loose I resoldered shorter connections and used hotglue/double side tape to fit everything in. Here the layout I choose to do: 


![alt text](Top_View.PNG)

![alt text](car_side.PNG)


## **5. Lower Limit PWM **

Under load it took 60 PWM on both sides to get it moving. Wihtout load it took 40 PWM to get it spinning. To pivot in place I made onen side 70 PWM to go right and the other 70 PWM to go left as shown below: 



[![](https://markdown-videos-api.jorgenkh.no/youtube/yudRkV-ePfE)](https://youtu.be/yudRkV-ePfE)






