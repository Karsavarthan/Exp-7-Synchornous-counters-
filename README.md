# Exp-6 Synchornous counters up counter 
### AIM: To implement 4 bit up counters and validate  functionality.
### NAME:KARSAVARTHAN.R.R
### REG NO:23003628
### HARDWARE REQUIRED:  – PC, Cyclone II , USB flasher
### SOFTWARE REQUIRED:   Quartus prime
### THEORY 

## UP COUNTER 
The counter is a digital sequential circuit and here it is a 4 bit counter, which simply means it can count from 0 to 15 and vice versa based upon the direction of counting (up/down). 

The counter (“count“) value will be evaluated at every positive (rising) edge of the clock (“clk“) cycle.
The Counter will be set to Zero when “reset” input is at logic high.
The counter will be loaded with “data” input when the “load” signal is at logic high. Otherwise, it will count up or down.
The counter will count up when the “up_down” signal is logic high, otherwise count down

Since we know that binary count sequences follow a pattern of octave (factor of 2) frequency division, and that J-K flip-flop multivibrators set up for the “toggle” mode are capable of performing this type of frequency division, we can envision a circuit made up of several J-K flip-flops, cascaded to produce four bits of output.
The main problem facing us is to determine how to connect these flip-flops together so that they toggle at the right times to produce the proper binary sequence.
Examine the following binary count sequence, paying attention to patterns preceding the “toggling” of a bit between 0 and 1:
Binary count sequence, paying attention to patterns preceding the “toggling” of a bit between 0 and 1.

Note that each bit in this four-bit sequence toggles when the bit before it (the bit having a lesser significance, or place-weight), toggles in a particular direction: from 1 to 0.



 
 

Starting with four J-K flip-flops connected in such a way to always be in the “toggle” mode, we need to determine how to connect the clock inputs in such a way so that each succeeding bit toggles when the bit before it transitions from 1 to 0.

The Q outputs of each flip-flop will serve as the respective binary bits of the final, four-bit count:

 
 

Four-bit “Up” Counter
![image](https://user-images.githubusercontent.com/36288975/169644758-b2f4339d-9532-40c5-af40-8f4f8c942e2c.png)



### Procedure

### PROGRAM FOR UPCOUNTER
![image](https://github.com/Karsavarthan/Exp-7-Synchornous-counters-/assets/139841970/96414469-cda6-4fd7-83be-6f22ea63d770)

### RTL LOGIC UP COUNTER ![image](https://github.com/Karsavarthan/Exp-7-Synchornous-counters-/assets/139841970/f00bd097-6171-4305-aaa2-2e51d48b4ba6)

### TIMING DIGRAMS FOR UPCOUNTER  ![image](https://github.com/Karsavarthan/Exp-7-Synchornous-counters-/assets/139841970/f48765de-a810-4a67-b438-cb2cbefe3e3b)

### TRUTH TABLE 
![image](https://github.com/Karsavarthan/Exp-7-Synchornous-counters-/assets/139841970/1e3dd63a-15b7-4243-9aba-79a728dd8bbe)


### RESULTS To design Synchornous counters up counter 
