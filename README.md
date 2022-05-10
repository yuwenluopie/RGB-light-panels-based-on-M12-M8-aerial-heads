# RGB-light-panels-based-on-M12-M8-aerial-heads
This is an **RGB** fill light for a camera and consists of two pieces: the switch connection board and the light board.<br>
We would like to implement the control of the colour and start/stop of the light beads in different areas of the light module by sending the corresponding code commands via **RS232 communication**. The colour range of the beads can be controlled by the corresponding commands, with RGB colours adjustable and flashing or constant light.<br>
## Function Detail
17 groups of beads<br>
The parameters of each group of beads can be set by sending a command<br>
Mask values in the range 0-255 <br>
Brightness value range is 0-255<br>
R-value range 0-255<br>
G-value range is 0-255 <br>
B-value range is 0-255<br>
The time range is 0-255 ms<br>
The start/stop status of each group of beads can be set by sending the command<br>
Flashing<br>
Off<br>
Flashing mode: red light green light yellow light red light flashing green light flashing red and green light alternately
Working status of the overall light source: one signal must be always on when the light source is working and the working status of the overall light source can be queried by sending a command

### Switch connection
The switch is powered by an M8 M12 header and connects to the network cable as well as the IO, the pin definition is shown in the diagram below <br>
![interface of Switch](https://user-images.githubusercontent.com/88228465/167525843-a663d5e4-9d15-40c4-a2dc-18d86da3fb58.png)<br>
![dimensions of Switch](https://user-images.githubusercontent.com/88228465/167525902-676b74cd-2b8c-41ea-9be2-58fced4ea768.png)<br>
4P switch power reserve --- 4 core port size is 7*5mm     Quantity 1<br>
6P camera power and IO reservation --- 6 core port size is 10*5mm     Quantity 4<br>
8P switch communication reserve position -----8 core port size is 15*5mm    Quantity 1<br>
The specific position is subject to the convenience of adding light wiring<br>
The thickness of the board is 5mm<br>
Camera and switch power supply voltage is 12V<br>
The camera IO port is not wired directly out <br>
<br>
The camera IO port :<br>
![The camera IO port](https://user-images.githubusercontent.com/88228465/167526194-c1f0dac6-6fe9-475b-a302-1f4dc67db7ed.png)<br>

The 6 wires of the light source are power + - ground RS232 three communication wires<br>
M12 12-pole plug power and IO cable Definition<br>
1 Power supply + 12V<br>
2 Power supply Negative<br>
3 232 communication RXD<br>
4 232 communication TXD<br>
5 232 communication GND<br>
6 Ground<br>
7 ---<br>
8 ---<br>
9 ---<br>
10 ---<br>
11 ---<br>
12 ---<br>
Access to mains power<br>
Power the 6P lines of each of the three cameras.<br>
The power cables of the three cameras are to supply power to their respective indicator lights, which light up when the cameras are powered up<br>
The power cable of the switch is to power the switch indicator, the switch is powered and the indicator is on<br>
![image](https://user-images.githubusercontent.com/88228465/167538234-168fd1f9-8a19-4308-b03f-cdb4b5f59f9c.png)

### Light Board
The dimensions of the connection board are 80mm radius a cricuit<br>
For details of the light change modes please read the document "Lightmode".<br>

