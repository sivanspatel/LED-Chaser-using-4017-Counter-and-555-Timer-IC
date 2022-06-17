**# LED-Chaser-using-4017-Counter-and-555-Timer-IC**

You must have seen different kinds of decoration lighting patterns. In this LED chaser circuit, we have created an interesting LED blinking pattern by using a 555 timer IC and Counter IC CD 4017.

**Required Components**
CD 4017 Counter
555 Timer IC
150, 1K, 10K Resistors
10K Variable Resistor
10uf, 100nF capacitor
Breadboard
9 Volt Battery
LED

**Circuit Diagram and Explanation**
![image](https://user-images.githubusercontent.com/71811374/174324801-02b68408-ecff-4de1-b28f-d5ff8a05ba1b.png)

When we power the circuit, LEDs start glowing one by one for a defined time period. Means first LED Q1 glows and then Q2 glows and Q1 turned OFF and then Q3 glows and Q2 turned OFF and so on. When we change resistance of variable resistor then speed of LED’s increase. Because frequency of 555 timer increases and this increases frequency signal is directly connected to counter’s trigger pin. So that counter changes its state faster.

555 timer frequency formula:

The charge time (output HIGH) is given by :

T1 = 0.693 (R1 +VR) C1

The discharge time (output LOW) by :

T2 = 0.693 (R2) C1

Thus the total period T is given by :

T = T1 + T2 = 0.693 (R1 + 2VR) C1

The frequency of oscillation is:

F= 1/T

F=1.44/(R1+2VR)C1

The main part of this LED chaser circuit diagram is 555 timer IC which generates some variable frequency. 555 timer IC is a general purpose IC which can be configured in some different modes like Astable, Monostable and Bistable. Here in this project we configured 555 timer as an Astable multivibrator in which both the stages of signal are unstable. Some time we call frequency generator also. Here we use output signal of this Astable multivibrator to trigger IC CD 4017 counter to change its state to perform desired task.

Here we have connected 555 timer IC in Astable mode for generating a trigger pulse of some time period. A variable resistor is connected for changing the cycle frequency of 555 timer’s output. A CD4017 counter IC is also connected with this circuit for lighting LEDs. 10 red LED’s are connected to Q0-Q9 pin (pin 3) through 150 ohm resistor. MR pin (pin 15), enable or clock inhbit pin (pin 13) is directly connected with ground and Clock pin of counter directly connected with output pin of 555 Timer.
