# AUTOMATED PLANT INCUBATOR
Design an automated plant incubator with Raspberry Pi
We are make a Automated Plant Incubator based on the Raspberry Pi. The green plants can make people feel relaxing and comfortable, but there are many people become busier and busier. This kind of people are too busy to take care of their plants. This kind of Automated Plant Incubator can help them to automatedly take care of the plant which in the incubator. The Automated Plant Incubator can help people take care of the plant, and this incubator can show the environment detial of the incubator in a small screen. The user can see the environment detail in the screen and they can also change the incubator's parameters by touch the screen. This incubator is aim to help those busy people to water and take care of their plant automatedly.

### SYSTEM DESCRIPTION

The first sensor what used is DHT11 temperature and humidity sensor to measure the incubator's environment temperature and humidaty. The second on is YL-69 soil humidity sensor, this sensor will work with a small water pump. We plan to set a range of the soil humidity in the program, when the soil's humidity is lower than the range, the water pump will be turned on, to water the plant, when the humidity in this range the water pump will be stoped. After that, we add a light intensity sensor GY-30 and a small case fan in this incubator, the small case fan is used to keep the incubator vented. All of the sensors will give the data to the Raspberry PI, and the Raspberry will show all the data in a screen. We plan to design a GUI, and it will allow the user to change the incubator's parameter by mouse. 
At last, we think about the plant uneven illumination. We plan to use photoresistence and a motor to make a system like the following picture:

![alt text](https://github.com/Kenny840394191/Automated-Plant-Incubator/blob/master/Motor.png)

The incubator will be put in the foundation. And it will pinwheel with the foundation based on the light intensity.

### BLOCK DIAGRAM

![alt text](https://github.com/Kenny840394191/Automated-Plant-Incubator/blob/master/Block%20Diagram.png)

### CONNECTION DIAGRAM

![alt text](https://github.com/Kenny840394191/Automated-Plant-Incubator/blob/master/Connection%20Diagram.png)

Then we will design a PCB according to the connection diagram.


### 5V 1Channel Relay
![alt text](https://github.com/Kenny840394191/Automated-Plant-Incubator/blob/master/5V%201Channel%20Relay.jpg)

I this project, we need to drive a motor and a small water pump. 
First the motor cannot be driven by the Raspberry Pi directly, so a 5V 1 channel relay will be added between the motor and the Raspberry Pi. Actuaaly the 5V 1 channel relay model will be used as a transistor between the motor and the Raspberry Pi.

In fact the main function of the 5V 1 channel relay model is boosted the voltage. The reason why we use the relay is the water pump can only be driven by 12V, but the Raspberry Pi only can supply 5V. Therefore we decided to use the relay model to boost the 5V to 12V to drive the small water pump. 
![alt text]()
