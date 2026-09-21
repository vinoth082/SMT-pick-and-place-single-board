# SMT-pick-and-place-single-board
# Aim:

To automatically pick and  place the SMD electronic components onto a single bare PCB accurately using an SMT pick-and-place machine.

# Apparatus required:

1.Pick and Place machine <br>
2.Components <br>
3.Single Bare board with solder paste<br>

# Procedure:

Step 1 : Switch ON the machine ,once  its opened there will be a PROJECT TAB in the tool Bar ,Click ON PROJECT ,then open CREATE PROJECT.<br>
Step 2: Save the file as per your project name.<br>
Step 3: Once you Saved the project you will find a (IMPORT PCB FILE) in the Screen , Click ON it.<br>
Step 4: Click on IMPORT DATA.<br>
Step 5 : Import your CSV file to the datasheet.<br>
Step 6: Edit the path name as per the Ref Description.<br>
Step 7: Delete the extra columns and rows available in the datasheet.<br>
Step 8: Remove the enable for  PRECISION MODE , which is available at the bottom of the screen. Once you disabled  the step 3 & Step 4 will be disappear.<br> 
Step 9 : Keep the PCB Board in the track of  Pick & Place Machine.<br>
Step 10 : Click on IN BOARD ,then the board in the track will automatically lock in the centre of the machine.<br>
Step 11: Set the value & assume the S1 and S2 therefore S1 - Top Left Corner Component and S2 - Bottom Right Corner component.<br>
Step 12 : In the bottom we can see the sign of the machine (XY) Set values are blank with Black boxes.<br>
Step 13: Save the file and move the joystick accordingly to the Point value of PCB board present in the track and set the value of S1 and S2. <br>
Step 14 : Click on Generate PCB Data.<br>
Step 15 : PCB direction should be same as imported Data ,then only we will be able to set the correct data ,otherwise we cannot able to fetch the exact values of data.<br>
Step 16: If the imported data value are in perfect match will get data like as picture shown below.<br>
Step 17: If the XY values are mismatching then adjust the board accordingly with joystick and update the correct XY values.<br>
Step 18 : Now set the values for MASK setting.<br> 
Step 19 : In mask setting > Set the values for F1 & F2.<br>
Step 20 : Fix the values for F1 & F2 as we before done for S1 & S2  and save the mask Setting data and close the window.<br>
Step 21 : Click on Optimize tab in the tool bar, you will get the window opened.<br>
Step 22 : Set the values for provider as shown in the figure.<br>
Step 23 : Set the values for noz as shown in the figure.<br> 
Step 24 : Set the values for Camera as shown in the figure.<br>
Step 25 : Set the values for Loop mode by setting its standard  for visual as shown in the figure and this window.<br> 
Step 26 : open > Optimize you will get the window page like as picture shown below with your given data.<br>
Step 27 : After closing the optimize window you will get the final PCB BOARD placed data will be shown as in picture.<br>
Step 28 : Click on Feeder Plug , Set the feeder point to the provider number given and load the feeder accordingly and click the check list  one by one as given.<br>
Step 29 : Now the set Feeder for our above feeder values mentioned like FEEDER (20,21,23,26).Now Feeder 20 : Go to Pick cord XY , the camera present in the nozzle will display the position, if needed adjust the frame accordingly , Click feeder and save the pick Cord XY and update the feeder.Same steps to be followed for all the feeder of 21,23 & 26.<br>
Step 30 : For Scanning process go to Feeder point 20 > Click on pick to fast cam.<br> 
Step 31: If there is any mismatch occurred during Scanning Process we want to tune accordingly to its respective nozzle.<br>
Step 32: Click on Diagnosis tab ,you will find a tab with Zero Errors ,(If its with Zero error now our process can do further final out,if there is an error occurs we have to clear accordingly as shown in figure .<br>
Step 33: Click on SMT RUN >SMT Setting >IS MOUNT >Enable all the boxes under Provider >Start > Auto run.<br>
Step 34 : Now the Machine is  all set to Run .<br>

# Theory

## Introduction
The SMT Pick and Place Machine is one of the most critical elements of the Surface Mount Technology (SMT) production line, responsible for accurately mounting electronic components on PCBs after solder paste printing. The ETS SMT MATE-660 SMT pick-and-place system is a highly efficient and reliable machine designed for medium-to-high throughput production with excellent placement accuracy. It automates the process of component handling, orientation, and placement, reducing manual intervention and improving overall product quality and manufacturing speed. In modern electronics, components have become more miniature and densely packed, such as QFN packages, BGAs, 0201/0402 passives, and fine-pitch ICs, which cannot be handled using manual tweezers or even semi-automated tools. The ETS SMT MATE-660 SMT enhances manufacturing productivity by offering high-speed placement, intelligent component recognition, and strong repeatability. It is widely used in industrial production, R&D facilities, and educational institutions because of its user-friendly interface, stable mechanical structure, and capability to process multiple PCB designs with high precision. This machine forms the backbone of printed circuit assembly lines by providing consistent, fast, and error-free component placement, ensuring the foundation of reliable circuit performance after reflow soldering.
## Construction and Components
The ETS SMT MATE-660 SMT pick and place machine is constructed with a rigid, vibration-free frame to maintain alignment and precision during high-speed operation. At the center of the machine is the XY gantry motion platform, powered by high-resolution servo motors and linear guides for accurate nozzle positioning. The component placement head is fitted with multiple vacuum nozzles to pick and place several components sequentially. The nozzles rotate to correct component orientation based on the inspection feedback system. The feeder banks are positioned in front of or on both sides of the machine and hold different packaged components supplied in tape reels, tubes, and trays. These feeders allow automatic, continuous dispensing of components, ensuring uninterrupted production. The machine’s vision inspection system includes upward-looking and downward-looking cameras. The downward camera helps in PCB fiducial recognition to correct alignment based on the programmed coordinates, while the upward camera reads component markings to verify size, polarity, pin orientation and detect any pickup offset. The PCB conveyor system carries the PCB inside the working area, centers it using side clamps, and locks it in position during placement. The control unit and software interface form the core of machine operation, enabling the import of PCB coordinate files, CAD/Gerber placement data, and feeder mapping for automated programming. The vacuum pump and pneumatic system provide suction pressure required for picking the components and releasing them accurately on the PCB pads. LED lighting, safety enclosures, ESD control, and error detection sensors support safe and reliable working conditions. All these components are integrated to achieve precise, high-speed pick and place performance.

<img width="712" height="606" alt="image" src="https://github.com/user-attachments/assets/0752d9a0-67f0-4e0d-b3f7-e97b0100b5b0" />


## Working and Operation
The working of the ETS SMT MATE-660 SMT pick and place machine follows a sequential flow of intelligent component placement programming and automated physical operations. The process begins with loading the PCB onto the conveyor platform, where it is clamped and fixed in a steady position. The machine identifies fiducial marks on the PCB using the downward camera and aligns the PCB coordinates to eliminate any mechanical tolerance or misalignment. Meanwhile, the operator assigns each component type to its corresponding feeder slot through the software interface. Once the setup is complete, the placement cycle begins. The placement head moves to the feeder bank, and the vacuum nozzle picks a specific component from the reel feed. The upward camera inspects the picked component to ensure proper size, polarity, and orientation. If the orientation is not correct, the nozzle automatically rotates the component to the required angle. The gantry system moves the placement head precisely to the PCB pad location, and the nozzle places the component on the solder paste. During this process, the machine constantly tracks speed, nozzle height, pickup force, and placement accuracy to enhance repeatability. The placement continues for all programmed components, covering passives, IC packages, connectors, LEDs, sensors, and other SMD devices. After the placement cycle is completed, the PCB exits the conveyor and moves to the next stage—typically the reflow oven for soldering. The machine automatically pauses when it detects errors such as missing components, feeder jams, vacuum failure, or misaligned pickup. The operator can resume the job after fixing the issue without disturbing the rest of the placement cycle. This high level of operational automation ensures maximum accuracy and throughput while reducing human fatigue and time consumption.

## Functions and Features 
1.	High-precision automatic component placement – The machine ensures micrometer-level placement accuracy using dual-camera vision inspection for both PCB alignment and component orientation, reducing placement errors and guaranteeing strong solder joints after reflow.<br>
2.	Multi-nozzle pick head with automated feeder compatibility – Several nozzles work simultaneously to pick and place different component sizes, significantly increasing placement speed and supporting high-density PCB designs.<br>
3.	Smart software with CAD/Gerber import and error detection – The system supports automatic programming by importing placement data directly, while in-built diagnostic alarms help identify feeder jams, pick-up errors, missing components, and misalignment.<br>
4.	Component rotation and height control – Each component automatically rotates to the correct polarity and angle while the nozzle height adjusts according to the package profile, enabling accurate handling of tiny passives and high-pin-count ICs.<br>
5.	Stable mechanical structure with continuous production capability – The rigid frame, smooth servo motion control, and optimized conveyor mechanism allow continuous operation for long production runs without calibration drift.<br>

## Application:
1.	Industrial electronics manufacturing – Used for mass production of consumer electronics, power modules, smart devices, and embedded hardware where fast and accurate SMD assembly is required.<br>
2.	Prototype development and R&D labs – Ideal for testing new circuit designs where frequent modifications and short production runs are common.<br>
3.	Educational institutes and training centers – Used for teaching SMT assembly and automated manufacturing concepts to engineering and diploma students.<br>
4.	Automotive and aerospace electronic systems – Helps manufacture high-reliability PCBs such as control modules, safety sensors, communication interfaces, and advanced driver-assistance circuits.<br>
5.	IoT and medical device production – Supports ultra-compact PCB designs for wearables, biomedical sensors, wireless nodes, and miniature embedded systems requiring micro-sized components and fine-pitch ICs.<br>

# Output

## Bare PCB board

<img width="810" height="801" alt="image" src="https://github.com/user-attachments/assets/4c93caea-e07f-431c-a12c-5d7bb43649ac" />



## Bare PCB board with components
<img width="792" height="947" alt="image" src="https://github.com/user-attachments/assets/53f98ca5-98db-4339-b0c9-efa76ac18174" />





# Result
The SMT pick-and-place machine successfully identified, picked, and placed the SMD electronic components onto the bare PCB with high positional accuracy. Component alignment, orientation, and placement quality were consistent across all test points. Misplacements and rotation errors were minimal, demonstrating effective vision-assisted positioning and reliable nozzle performance. Overall, the experiment confirms that the pick-and-place machine achieves precise, repeatable, and
fully automated component placement, making it suitable for high-quality SMT assembly.

