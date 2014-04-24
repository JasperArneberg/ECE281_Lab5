ECE281_Lab5
===========

Lab 5: PRISM

#Program 1

##Overall Description

Below is the simulation waveform for Program 1.

![alt text](https://github.com/JasperArneberg/ECE281_Lab5/blob/master/entire_waveform.png?raw=true "Entire Waveform")

This program starts with the number 9, and it continually adds 1 to it until it reaches the value of 0. At this point, the program does no more operations, and the output stays at 0. 

##Close Analysis

We can analyze the waveform close up to see what is going on. Each command is shown below. 

###LDAI 8
![alt text](https://github.com/JasperArneberg/ECE281_Lab5/blob/master/ldai8.png?raw=true "LDAI 8")

The first 10 nec is the Fetch command, and then decode and immediate execute follow.

###ADDI 1
![alt text](https://github.com/JasperArneberg/ECE281_Lab5/blob/master/addi1.png?raw=true "ADDI 1")

The first 10 nsec is the Fetch command, and then decode and immediate execute follow.

###OUT 3
![alt text](https://github.com/JasperArneberg/ECE281_Lab5/blob/master/out3.png?raw=true "ADDI 1")

The first 10 nsec is the Fetch command, and then Decode, Decode LoAddr, and Direct IO Execute follow.

###JN Loop
![alt text](https://github.com/JasperArneberg/ECE281_Lab5/blob/master/jnloop.png?raw=true "JN Loop")

The first 10 nsec is the Fetch comand, and then Decode, Decode LoAddr, Decode HiAddr, and Jump Execute follow.

#Program 2

##Flow Chart
Here is a flow chart for Program 2:
![alt text](https://github.com/JasperArneberg/ECE281_Lab5/blob/master/flow_chart.jpg?raw=true "Program 2 Flow Chart")

This program counts with two digits between 0 and 99. Once the end is reached, it wraps back around. When the first switch is on, it counts backwards.

#Demonstrations
| Functionality | Witness | Date | Time |
| :--: | :--: | :--: | :----: |
| Program 1 | Dr. Neebel | 22 April 2014 | 1340 |
| Program 2 PRISM | Dr. Neebel | 23 April 2014 | 1328 |
| Program 2 FPGA | Dr. Neebel | 23 April 2014 | 1329 |

#Documentation
C3C El-Saawy attempted to help me troubleshoot the first program, but Dr. Neebel eventually told the class what the problem was.
