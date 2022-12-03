# BuzzerHorn
A BuzzerHorn to Fit a Piezo Transducter, 12.2mm x 6.5mm on the GPAD.  
A FreeCad project.  

### Buzzer horn on GPAD assembly
![image](https://user-images.githubusercontent.com/5836181/204543966-32a35c15-1148-4263-9631-23105a5c4b57.png)

### First Test Results 20221202
Test on DUT serial numbers 2.  
Tested with GPAD version 0.03 Firmware.
Version 0.3 firm ware sets the following frequencies for alarms a0 to a5.
>const int BUZZER_LVL_FREQ_HZ[]= {0,128,256,512,1024,2048};

Measurment was made verticaly above the DUT. The DUT was placed on a table top with the transducer pointed up. So the measurement was on axis. 
Forrest noticed that he could hear Alarms at A2 which he did not hear before.  
Measure SPL at A0-A5 with and with out the BuzzerHorn.  
Tested at 10cm from transducter. No enclosure.  
Here is a plot of the amplitude as measreud by TBD SPL meter.  
![./measurements/spl-graph-conev3.png](./measurements/spl-graph-conev3.png)
Note althought the measured SPL for with Buzzer Horn was lower on axis the buzzer could be heard off axis perhaps better.

### Tagged Version Descriptions
I have made several guesses at shapes to try each time making tweeks for fit to GPAD Version 1 PCB.

Version 3.0  
![image](https://user-images.githubusercontent.com/5836181/204536651-52f1deb7-3420-41a9-9ea4-b9a47d4a39b4.png)
Version 3.0 Reduce top diamter to about 0.6 inch so will not interfer with LED D201 on GPAD.

Version 2.0  
![image](https://user-images.githubusercontent.com/5836181/204439320-8172296c-358a-48d1-b215-9bfff2cb0830.png)  
With fillet at appature.

Version 1.0  
![image](https://user-images.githubusercontent.com/5836181/204424521-fbb57517-f856-442d-b4ad-dd70aa9b67e2.png)  
Sharp corner at appature.

### Buzzer Information
This horn is designed for a buzzer part I found at JLCPCB: **https://jlcpcb.com/partdetail/Tdk-PS1240P02BT/C76871**  
Data sheet for buzzer at: **https://datasheet.lcsc.com/lcsc/1811032111_TDK-PS1240P02BT_C76871.pdf**  
![image](https://user-images.githubusercontent.com/5836181/204526125-bdc29536-359c-43d1-9c7f-f91dde45fbc8.png)

# Slicer project and GCODE
A PrusaSlicer Project file containing various rotations, as well as generated gcode from the same.
