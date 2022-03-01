# Ring_VCO <br/>
A voltage-controlled oscillator is an electronic oscillator whose oscillation frequency is controlled by a voltage input. The applied input voltage determines the instantaneous oscillation frequency. This circuit includes a 3-stage ring oscillator, Buffer and a bias generator.
# Table Of Content <br/>
* [Abstract](https://github.com/Mahima-Goyen/Ring_VCO#abstract)<br/>
* [Reference Circuit Diagram](https://github.com/Mahima-Goyen/Ring_VCO#reference-circuit-diagram)<br/>
* [Schematic](https://github.com/Mahima-Goyen/Ring_VCO#schematic)<br/>
* [Expected Results](https://github.com/Mahima-Goyen/Ring_VCO#expected-results)<br/>
* [Simulation Results](https://github.com/Mahima-Goyen/Ring_VCO#simulation-results)<br/>
* [Netlist](https://github.com/Mahima-Goyen/Ring_VCO#netlist)<br/>
* [Author](https://github.com/Mahima-Goyen/Ring_VCO#author)<br/>
* [Acknowledgements](https://github.com/Mahima-Goyen/Ring_VCO#acknowledgements-)<br/>
* [Reference](https://github.com/Mahima-Goyen/Ring_VCO#reference-)<br/>
# Abstract<br/>
A conventional VCO has different structural and performance parameters due to its wide range of applications in various environmental conditions.The basic circuit structure of this study is designed and implemented using the symmetrical load differential VCO structure, because it has many advantages. The design is implemented using Synopsys tool using 28nm technology node. 

# Reference Circuit Diagram<br/>
![image](https://user-images.githubusercontent.com/100615611/156039758-b97fe2d3-df31-4414-80a2-adbbf0a73d95.png)<br/>
*Figure 1 - Delay Circuit*<br/>
There are two circuit blocks added to design the new differential VCO extension. The first one is called the swing enhanced block and the second is called self-excitation tube.
The voltage control technique uses the body bias voltage of the nMOS transistor, which in turn changes the voltage threshold of the transistor.
<br/>
![image](https://user-images.githubusercontent.com/100615611/156039714-a9fbcf1c-9ff4-40f3-b960-41adcdeaa7e4.png)<br/>
*Figure 2 - 3-stage VCO*<br/>
In this work, a 3-stage ring oscillator is used where each stage is a modified version of the differential symmetrical load delay. 

# Schematic<br/>
1. BIAS GENERATOR<br/>
![image](https://user-images.githubusercontent.com/100615611/156038092-6860b2ff-21f1-4249-98bd-b2f4a02284a0.png)<br/>
*Figure 3 - Bias Generator*<br/>
2. BUFFER<br/>
![image](https://user-images.githubusercontent.com/100615611/156038179-7b9d7eec-75fd-4b44-9309-eaf4d8c5738e.png)<br/>
*Figure 4 - Buffer Circuit*<br/>
3. DELAY CELL<br/>
![image](https://user-images.githubusercontent.com/100615611/156038295-6f0fdbb5-7f11-469c-9573-0c8d27874c1b.png)<br/>
*Figure 5 - Delay Circuit*<br/>
#Symbols<br/>
1. BIAS GENERATOR<br/>
![image](https://user-images.githubusercontent.com/100615611/156039313-e4307be1-119e-4c82-a803-251dd4bcec24.png)<br/>
*Figure 6 - Bias Generator Symbol*<br/>
2. BUFFER<br/>
![image](https://user-images.githubusercontent.com/100615611/156039223-11dfd259-751b-4050-917e-2ed1c9c075b1.png)<br/>
*Figure 7 - Buffer Symbol*<br/>
3. DELAY CELL<br/>
![image](https://user-images.githubusercontent.com/100615611/156039128-a4f74664-d315-4f92-97d1-2c5558417675.png)<br/>
*Figure 8 - Delay Cell Symbol*<br/>
4. TEST BENCH<br/>
![image](https://user-images.githubusercontent.com/100615611/156037769-a591f095-72a9-468d-867a-aee673031abe.png)<br/>
*Figure 9 - Test Bench Circuit*<br/>
Where Vctrl = 0.9 V (It can be changed to control the output Voltage accordingly)<br/>
Initial input voltage = 1 V<br/>
Vdc = 0.8 V

# Expected Results<br/>
 ![image](https://user-images.githubusercontent.com/100615611/156039589-03cb4df2-13ad-4a0a-a967-7adb32fa27a3.png)<br/>
 *Figure 10 - Expected Transient Response*<br/>
# Simulation Results<br/>
![image](https://user-images.githubusercontent.com/100615611/156037458-8d2a0176-1520-4656-9c09-4add9b52e469.png)<br/>
The oscillation settles between 0.2 and 0.9 Volt
 *Figure 11 - Transient Response*<br/>
![image](https://user-images.githubusercontent.com/100615611/156037683-b11efbf3-a1bb-4d5c-a22a-fea69efabdd8.png)<br/>
 *Figure 12 - Transient Response (Zoomed Out)*<br/>
<br/>(*Other types of results can be taken to measure the phase noise,oscillation frequemcy - But purpose of this simulation was to create only a modified VCO*)<br/>
# Netlist<br/>
You can view the circuit netlists [here](https://github.com/Mahima-Goyen/Ring_VCO/blob/main/Netlist)<br/>
# Author<br/>
Mahima Goyen<br/>
# Acknowledgements <br/>
[Kunal Ghosh, Co-founder, VSD Corp. Pvt. Ltd.](https://www.linkedin.com/in/kunal-ghosh-vlsisystemdesign-com-28084836/)<br/>
[Cloud Based Analog IC Design Hackathon](https://www.iith.ac.in/events/2022/02/15/Cloud-Based-Analog-IC-Design-Hackathon/)<br/>
[Synopsys India](https://www.synopsys.com/)<br/>
# Reference <br/>
https://ieeexplore.ieee.org/document/8268826 <br/>
