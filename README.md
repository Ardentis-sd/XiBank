# XiBank

<p>
<img src="https://img.shields.io/badge/CAD-Altium-blue"> 
<img src="https://img.shields.io/github/repo-size/Ardentis-sd/XiBank"> 
<img src="https://img.shields.io/youtube/views/kC_nnOEB7hU?style=social">
</p>

XiBank is a controller board that designed to fit into Mi Power Bank enclosure and replace the original board in case it has become malfunction or non-repairable. 

<p>
<img width="500" alt="TopView_XiBank_V1.0.png" src="https://github.com/Ardentis-sd/XiBank/blob/main/Pictures/TopView_XiBank_V1.0.png">
<img width="500" alt="BottomView_XiBank_V1.0.png" src="https://github.com/Ardentis-sd/XiBank/blob/main/Pictures/BottomView_XiBank_V1.0.png">
</p>

### Features:
 - Board shape and sizes, mount holes and connectors placement are identical to original board.
 - 1x USB Micro input port, 2x USB Type A ouput ports.
 - Simple 1mm 2-layer board.
 - IP5328P utilized SOC (support 5V, 9V, 12V voltage input and 3.1A@5V, 2.0A@9V, 1.5A@12V output current capacity).
 - The smallest component case is 0603.
 - Low components count.

### Known Issue:
 - IP5328P for some reason don't like the Baseus "BS-EU905" quick charger. In  my case when battery become charged to 100% there is no suspend 
event and Baseus charger cyclycaly reconnects to IP5328P, thus 4th LED always blinkink and there is no chance to understand that battery is full.
Moreover this situation damaging the internal high-side MOSFET of IP5328P's synchronous switch and "VSYS" andd "LX" pins become shorted.

### Video:
[![Second Life For Xiaomi Power Bank](https://img.youtube.com/vi/kC_nnOEB7hU/0.jpg)](https://youtu.be/kC_nnOEB7hU)
