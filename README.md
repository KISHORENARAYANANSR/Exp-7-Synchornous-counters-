# Exp-6-Synchornous-counters - up counter and down counter 
### AIM: To implement 4 bit up and down counters and validate  functionality.
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



## DOWN COUNTER 

As well as counting “up” from zero and increasing or incrementing to some preset value, it is sometimes necessary to count “down” from a predetermined value to zero allowing us to produce an output that activates when the zero count or some other pre-set value is reached.

This type of counter is normally referred to as a Down Counter, (CTD). In a binary or BCD down counter, the count decreases by one for each external clock pulse from some preset value. Special dual purpose IC’s such as the TTL 74LS193 or CMOS CD4510 are 4-bit binary Up or Down counters which have an additional input pin to select either the up or down count mode.
![image](https://user-images.githubusercontent.com/36288975/169644844-1a14e123-7228-4ed8-81a9-eb937dff4ac8.png)


4-bit Count Down Counter
### Procedure
1.Create a new project in QuartusII software. 2.Name the project as uc for upcounter and dc for
down counter. 3.Create a new verilog hdl file in the project file. 4.Name the module as dc and uc for
down counter and up counter. 5.Within the module declare input and output variables. 6.Create a
loop using if-else with condition parameter as reset value. 7.End the loop. 8.End the module



### PROGRAM 

Program for flipflops  and verify its truth table in quartus using Verilog programming.
Developed by: KISHORE NARAYANAN S R
RegisterNumber:  23006250

## UP COUNTER:
![UPCOUNTER CODE](https://github.com/KISHORENARAYANANSR/Exp-7-Synchornous-counters-/assets/148202102/5fcd763a-3bee-43f8-ad7a-ff84fc3ab3f6)

## DOWN COUNTER:
![DOWNCOUNTER CODE](https://github.com/KISHORENARAYANANSR/Exp-7-Synchornous-counters-/assets/148202102/2e81e5d2-4774-4efe-bfd4-10bf282c5ec9)


## RTL LOGIC UP COUNTER AND DOWN COUNTER:
## UP COUNTER:
![UPCOUNTER RTL](https://github.com/KISHORENARAYANANSR/Exp-7-Synchornous-counters-/assets/148202102/e0dc8085-2bdb-4909-83b2-43250f6dbb17)

## DOWN COUNTER:
![DOWNCOUNTER RTL](https://github.com/KISHORENARAYANANSR/Exp-7-Synchornous-counters-/assets/148202102/85fa06b5-36f4-4384-8beb-b379d2fc2474)


## TIMING DIGRAMS FOR COUNTERS:
## UP COUNTER:
![UP TIME](https://github.com/KISHORENARAYANANSR/Exp-7-Synchornous-counters-/assets/148202102/9b17ca4a-30b5-4585-980c-9245f5d91ebd)

## DOWN COUNTER:
![THE REAL DOWN TIME](https://github.com/KISHORENARAYANANSR/Exp-7-Synchornous-counters-/assets/148202102/73f135f9-fc52-4e7a-837e-98170591dd43)

## TRUTH TABLE;
## UP COUNTER:
![UP TT TABLE](https://github.com/KISHORENARAYANANSR/Exp-7-Synchornous-counters-/assets/148202102/57fcc8ee-80b1-4a53-8ee3-c2691d16d8ff)

## DOWN COUNTER:
![DOWN TT](https://github.com/KISHORENARAYANANSR/Exp-7-Synchornous-counters-/assets/148202102/3edc48ea-4d45-42d0-9490-e62cc0144179)

## RESULTS :
Thus Synchornous counters up counter and down counter circuit are studied and the truth table for
different logic gates are verified.
