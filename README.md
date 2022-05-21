# Autonomous Plant Monitoring HAT for Discovery Board with STM32FC051
This repository will be updated at each stage of the design process, and where necessary changes are made.

# Group Members:
* Ryan Jones (JNSRYA006)
* Alex Cargill (CRGALE002)
* Devlin Trafford (TRFDEV001)

# Project Details
### This project is part a project for EEE3088F in 2022
This project will design a HAT *(Hardware Attached on Top)* for a STM Discovery Board which uses the STM32FC051. The use case for this HAT is for semi-autonomous indoor plant growing.  This design was created for small scale agricultural setups. Appropriate user stories were applied to develop the Specifications. Given these use cases, the PCB is able to:

* Monitor the **temperature** around a plant
* Get precise readings of the **light level** a plant is receiving. 

These measurements can then be used to integrate with a control system that can adjust the temperature and light that a plant receives. 

This device was thoroughly designed and the PCB has dimensions of: 96.01 mm x 70.01 mm, weighs ~0.11kg per board and costs $14.576 per board (excl. Shipping from JLCPCB).

### Concept of the project
The HAT will be used as a water sensing module for agricultural purposes. It will have a moisture sensor located in the soil that the plants are growing in and a flow rate sensor connected to the irrigation system. These sensors will connect to a STM Discovery board, which will act as the brain of the system. This system is for indoor autonomous growing setups which has applications in disruptive agricultural industries like marijuana growing. The HAT is intended to be used in small scale, home-setups in order to automate the watering of the plant as well as small-scale, industrial applications in an emerging market.

## Repository Structure
### Each sub-folder contains different aspects relating to different parts of the project
* PCB: The KiCAD Project, Schematics, PCB & Layout and Project Libraries
* Firmware: Any software developed for the hardware or instructions on where to find relevant sofware in cases where it makes more sense to have this in its own dedicated repo
* Docs: Project documentation, Draft documents, ERC & DRC reports, project handins, schematic screenshot & documents and component datasheets
* Production: The final gerber files, BOM, Budget, or anything required by the fabrication houses
* Simulation: Any simulation files (SPICE) or design stage generated results (matlab or excel) 
* CAD: Any 3D models or mechanical designs for enclosures or support


# Hardware Requirements


# Software Requirements

# How to connect the PCB to the STMDiscovery Board

# How to connect the PCB & STMDiscovery to your computer

# How to send your first data to the board!


# License
[Creative Commons Attribution 4.0 International license](https://choosealicense.com/licenses/cc-by-4.0/)
