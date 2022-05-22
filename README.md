# Autonomous Plant Monitoring HAT for Discovery Board with STM32F051x8
This repository will be updated at each stage of the design process, and where necessary changes are made.

# Group Members:
* Ryan Jones (JNSRYA006)
* Alex Cargill (CRGALE002)
* Devlin Trafford (TRFDEV001)

# Project Details
### This project is part a project for EEE3088F in 2022
This project will design a HAT *(Hardware Attached on Top)* for a STM Discovery Board which uses the STM32F051x8. The use case for this HAT is for semi-autonomous indoor plant growing. It will have a temperature sensor located as close to the plant as possible as well as a light sensor facing the main direction which the plant receives light from . These sensors will connect to a STM Discovery board, which will act as the brain of the system. This design was created for small scale agricultural setups. Appropriate user stories were applied to develop the Specifications. Given these use cases, the PCB is able to:

* Monitor the **temperature** around a plant
* Get precise readings of the **light level** a plant is receiving. 

See a 3D render of the PCB from KiCad below,

| ![PCB 3D Render](C:\Users\ryanj\OneDrive - University of Cape Town\Third Year\First Semester\EEE3088F\HAT\EEE3088F_HAT\Docs\Schematic Schreenshots\3D_Render.png) |
| ------------------------------------------------------------ |

## Repository Structure
### Each sub-folder contains different aspects relating to different parts of the project
* ***PCB:*** The KiCad Project, Schematics, PCB & Layout and Project Libraries
* ***Firmware:*** Any software developed for the hardware or instructions on where to find relevant sofware in cases where it makes more sense to have this in its own dedicated repo
* ***Docs:***  Project documentation, Draft documents, ERC & DRC reports, project handins, schematic screenshot & documents and component datasheets
* ***Production:*** The final gerber files, BOM, Budget, or anything required by the fabrication houses
* ***Simulation:*** Any simulation files (SPICE) or design stage generated results (matlab or excel) 
* ***CAD:*** Any 3D models or mechanical designs for enclosures or support
# Hardware Requirements
 * [ ] STMDiscovery Board with an STM32F051x8 μC
 * [ ] 1 x MicroUSB to USB-A Cable
 * [ ] 1x MiniUSB to USB-A Cable
 * [ ] 8x Male to Female Jumpers

# Software Requirements

 - [ ] Computer 
	 - *Windows, Linux or MACOS*
 - [ ] STM32Cube IDE
	 - [Download available online](https://www.st.com/en/development-tools/stm32cubeide.html#get-software)
 - [ ] PuTTY
	 - [Download available online](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html)

# How to short the UVLO circuit

- On the LHS of the board, remove resistor **R12 & R10** using pliers and twisting and pulling the resistors

- Q1 & IC1 (Circled in **Orange**) are the MOSFET & Op-Amp in the UVLO circuit that needs to be removed by soldering one end of a wire to the top pad (Pad 2) of R12 to the top pad (Pad 2) of R10 (Circled in **Green**)

  | ![UVLO_shorting](C:\Users\ryanj\OneDrive - University of Cape Town\Third Year\First Semester\EEE3088F\HAT\EEE3088F_HAT\Docs\Schematic Schreenshots\UVLO_shorting.png) |
  | :----------------------------------------------------------: |

  

# How to connect the power module to the rest of the board

- On the top, RHS of the board, solder a wire between **TP9** *OR* the **+3V** pin pad and the right hand pin of **J7**
  - This will connect the power from the power module to the rest of the circuit
- If connected correctly, when a battery is inserted or a USB is connected, a **Red** diode (**D9**) will turn on to indicate the sensing and microcontroller sub-circuits are receiving power.

# How to connect the PCB to the STMDiscovery Board

# How to connect the PCB & STMDiscovery to your computer

# How to send your first data to the board!


# License
[Creative Commons Attribution 4.0 International license](https://choosealicense.com/licenses/cc-by-4.0/)