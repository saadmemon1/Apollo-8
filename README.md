# Apollo-8 CPU in Logisim

## Overview

This repository contains the implementation of an 8-bit TOY CPU in Logisim. Apollo-8 is a simple computer with a minimal instruction set and 16 bytes of memory, and this project provides a Logisim simulation of its functionality.

## Table of Contents

- [Overview](#overview)
- [Getting Started](#getting-started)
    - [Prerequisites](#prerequisites)
- [Usage](#usage)
    - [Simulating in Logisim](#simulating-in-logisim)
    - [Loading Programs](#loading-programs)
    - [Running the CPU](#running-the-cpu)
    - [Viewing Memory](#viewing-memory)
- [Contributions](#contributions)
- [Acknowledgements](#acknowledgements)

## Getting Started

### Prerequisites

Make sure you have [Logisim](http://www.cburch.com/logisim/download.html) installed on your machine. Logisim requires Java 5 or later. If you do not have Java installed on your system, download it from [the Java website.](https://www.oracle.com/java/technologies/)

### Instruction Set
![Apollo-8 Reference Card.jpg](Apollo-8%20Reference%20Card.jpg)
### Usage
#### Simulating in Logisim
1. Open the Apollo-8.circ file in Logisim.
2. Navigate to the UI circuit to access the easy User controls.
3. Go to Simulate tab and enable Auto-Tick, and ideally set the Auto-Tick frequency to 2Hz. This controls the clock frequency for simulation.
#### Loading Programs
1. Disable Run button in the UI circuit.
2. Input the program by specifying the 4-bit address and 8-bit data.
3. Hold the LOAD button for a couple of seconds to load the specified value.
4. Repeat steps 2 and 3 for all the memory locations.
5. Press the Look button to see the contents of the memory.
#### Running the CPU
1. Ensure all the buttons in the UI circuit are disabled.
2. Disable auto-tick in the Simulate tab, and if the Clock is high, set it to low.
3. Enable the Run button.
4. Enable auto-tick and set the frequency to 2Hz.
5. The CPU will now start executing the program from the memory location 0.
6. The program will run until it reaches the HALT instruction or the end of the memory.
#### Viewing Memory
1. Turn the RUN pin off to stop the CPU.
2. Enter the address of the memory location to be viewed in the 4-bit address input.
3. Press the Look button to see the contents of the memory at that location.
## Contributions
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
## Acknowledgements
- [Logisim](http://www.cburch.com/logisim/) - A logic simulator which this project is based on.
- [TOY-8 CPU Reference Card](https://introcs.cs.princeton.edu/java/home/) - The instruction set for the CPU.