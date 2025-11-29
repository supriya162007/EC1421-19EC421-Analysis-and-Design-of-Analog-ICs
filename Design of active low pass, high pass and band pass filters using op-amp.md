# EC1421-19EC421-Analysis-and-Design-of-Analog-ICs
# DESIGN OF ACTIVE LOW PASS,HIGH PASS AND BAND PASS FILTERS USING OP-AMP 

## AIM: 

To design and obtain the frequency response of 
i) First order Low Pass Filter (LPF) 
ii) First order High Pass Filter (HPF) 
iii) Band pass filter
 
## APPARATUS REQUIRED

<img width="625" height="170" alt="image" src="https://github.com/user-attachments/assets/900fc8b3-3a8c-4208-bf52-98cc9e281e21" />

## THEORY
## LOW PASS FILTER 
 A LPF allows frequencies from 0 to higher cut of frequency, fH.  At fH the gain is 0.707 
Amax, and after fH gain decreases at a constant rate with an increase in frequency.  The gain 
decreases 20dB each time the frequency is increased by 10.  Hence the rate at which the gain 
rolls off after fH is 20dB/decade or 6 dB/ octave, where octave signifies a two fold increase in 
frequency.  The frequency f=fH is called the cut off frequency because the gain of the filter at this 
frequency is down by 3 dB from 0 Hz.  Other equivalent terms for cut-off frequency are -3dB 
frequency, break frequency, or corner frequency.
# HIGH PASS FILTER 
The frequency at which the magnitude of the gain is 0.707 times the maximum value of 
gain is called low cut off frequency.  Obviously, all frequencies higher than fL are pass band 
frequencies with the highest frequency determined by the closed –loop band width all of the op
amp. 
# BAND PASS FILTER 
A band pass filter has a pass band between two cutoff frequencies fH and fL such that fH > 
fL.  Any input frequency outside this pass band is attenuated.  There are two types of band-pass 
filters.  Wide band pass and Narrow band pass filters.  We can define a filter as wide band pass if 
its quality factor Q <10.  If Q>10, then we call the filter a narrow band pass filter.  A wide band 
pass filter can be formed by simply cascading high-pass and low-pass sections.  The order of 
band pass filter depends on the order of high pass and low pass sections.

## CIRCUIT DIAGRAM: 
## LOW_PASS
<img width="748" height="342" alt="image" src="https://github.com/user-attachments/assets/926e78ba-fc84-4bd6-b822-f8a42cb2c90d" />

## HIGH-PASS
<img width="779" height="318" alt="image" src="https://github.com/user-attachments/assets/76deb647-bc4e-45bb-8996-10dfbc0c260d" />

## BAND-PASS
![BF78419B-9FDF-475C-8560-6DF4E3FAE28F_4_5005_c](https://github.com/user-attachments/assets/1b5bddc7-0ac1-46ca-a2ed-cfa4f99e523f)

## MODEL GRAPH:
## LOW_PASS
<img width="779" height="318" alt="image" src="https://github.com/user-attachments/assets/94bfe11b-c3c5-42be-ad45-2191c82145d1" />

## HIGH-PASS
<img width="748" height="365" alt="image" src="https://github.com/user-attachments/assets/452e9e47-3e55-44f0-b24c-a6d8b7dbdf1c" />

## BAND-PASS
<img width="730" height="317" alt="image" src="https://github.com/user-attachments/assets/febe3aac-7ce9-41e6-aafb-4b88ab2fa040" />


## PROCEDURE - (LPF & HPF): 
1. Connect the circuit as shown in the circuit diagram. 
2. Select the corresponding cut-off frequency (higher or lower) and determine the value of C&R. 
select the value of R1 & Rf depending on desired passband gain Af.. 
3. Apply a constant voltage input sinusoidal signal to the non-inverting terminal of op-amp. 
4. Tabulate the output voltage Vo with respect to different values of input frequency. 
5. Calculate passband gain and plot the graph of frequency versus voltage gain & check the 
graph to  get approximately the same characteristic as shown in the model graph. 
# PROCEDURE:BAND PASS FILTER 
1. Select the lower and higher cut-off frequency and calculate the value of R & C for the given 
frequencies. 
2. Design for LPF & HPF separately and then combine the circuit by first placing the HPF 
followed by a LPF (i.e) HPF in series with LPF. 
3. Connect the circuit as shown in the circuit diagram. 
4. Apply a constant voltage input sinusoidal signal to the non-inverting terminal of op-amp. 
5. Tabulate the output voltage Vo with respect to different values of input frequency. 
6. Calculate passband gain and plot the graph of frequency versus voltage gain & check the 
graph to get approximately the same characteristic as shown in the model graph

## DESIGN:LPF & HPF:

<img width="429" height="324" alt="image" src="https://github.com/user-attachments/assets/b0f0ac0a-3006-494c-9096-e91ae2d6e87c" />

# DESIGN: BAND PASS FILTER
Design a BPF to pass a band of 400Hz to 2KHz with a pass band gain of 4.  
1. Select the highest cut-off frequency of LPF as fH = 10 KHz and the lowest cut-off frequency 
of HPF as fL = 1 KHz.  
2. Design the HPF first by taking fL = 1KHz. Assume the value of C < 1μf.  
Let C = 0.1μf.  
3. Calculate R from the expression.  
Given: fH = 2KHz  = 1/ (2πR1C1) 
   Let C1 = 0.1 µF, R1 = 7.9 KΩ 
Given: fL = 400Hz  = 1/ (2πR2C2) 
   Let C2 = 0.1 µF, R2 = 39.8 KΩ 
  Pass band Gain=4 
   Now   Ao = 1 + (Rf / R1)  
               2-1=(Rf / Ri) 
                Ri = Rf 
                 Let  Ri = Rf = 10 KΩ
## TABULATION:
## LOW_PASS
<img width="748" height="586" alt="image" src="https://github.com/user-attachments/assets/63676b94-30f1-4a49-9eb3-c75e8fb93dbc" />

## HIGH-PASS
<img width="779" height="544" alt="image" src="https://github.com/user-attachments/assets/c7c4caec-2260-422c-8f8f-24b137cf97ac" />

## BAND-PASS
<img width="730" height="502" alt="image" src="https://github.com/user-attachments/assets/cb8251e1-2881-4ff4-8ec3-281f195a23f9" />

## GRAPH:
## LOW_PASS
<img width="945" height="1280" alt="image" src="https://github.com/user-attachments/assets/20c905b3-69f1-4bed-ad93-7b25efa48b92" />

## HIGH-PASS
<img width="1600" height="1233" alt="image" src="https://github.com/user-attachments/assets/a9a6f162-d162-437c-8d0c-83bddc1af235" />

## BAND-PASS
<img width="944" height="1280" alt="image" src="https://github.com/user-attachments/assets/04eeb27b-ec95-4952-8ccc-c5fe1879b36a" />


 ## RESULTS:
Thus an Active Low pass, High pass and Band Pass Filters are designed and 
tested using op-amp IC 741. 

