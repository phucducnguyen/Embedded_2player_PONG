# PONG Game for 2 Players on Nexys A7 100T with Cortex-M0

## Project Overview

This project implements a classic two-player PONG game on the Nexys A7 100T FPGA board. The game logic is executed on an ARM Cortex-M0 processor, and the FPGA is programmed using Verilog. The provided Verilog files are sourced from ARM education. The project utilizes Xilinx Vivado for FPGA programming and Keil µVision 5 for Cortex-M0 development.

## Table of Contents

- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Hardware Setup](#hardware-setup)
- [Software Setup](#software-setup)
- [Building and Running the Project](#building-and-running-the-project)
- [Project Structure](#project-structure)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## Introduction

The PONG game is a simple but engaging project that demonstrates the integration of hardware and software components. Players control paddles on either side of the screen to bounce a ball back and forth. The game ends when a player fails to return the ball.

## Prerequisites

Before you begin, ensure you have the following:

- Nexys A7 100T FPGA board
- ARM Cortex-M0 processor
- Xilinx Vivado Design Suite
- Keil µVision 5 IDE
- ARM education Verilog files (provided in this project)
- USB cables for programming and power
- Basic understanding of Verilog and embedded C programming

## Hardware Setup

1. **Connect the Nexys A7 100T board** to your computer using the USB cable.
2. **Ensure the power jumper** on the board is set to the USB power option.
3. **Connect external components** (buttons, switches, and display) as needed for the PONG game controls.

## Software Setup

1. **Install Xilinx Vivado**: Download and install the Vivado Design Suite from the Xilinx website.
2. **Install Keil µVision 5**: Download and install Keil µVision 5 from the ARM website.
3. **Clone this repository**: Download the project files from the repository or clone it using Git.

```sh
git clone https://github.com/yourusername/pong-nexys-a7.git
```

## Building and Running the Project

### FPGA Programming with Vivado

1. **Open Vivado** and create a new project.
2. **Add the provided Verilog files** to the project.
3. **Configure the project** for the Nexys A7 100T board.
4. **Synthesize and implement the design**.
5. **Generate the bitstream** and program the FPGA.

### Cortex-M0 Programming with Keil

1. **Open Keil µVision 5** and create a new project.
2. **Add the provided C source files** to the project.
3. **Configure the project** for the Cortex-M0 processor.
4. **Compile the project** and ensure there are no errors.
5. **Load the compiled binary** onto the Cortex-M0 processor.

## Project Structure

The project directory is organized as follows:

```
pong-nexys-a7/
├── Application/
│   └── main.c                
├── Core/
│   ├── core_cm0.h
│   ├── core_cmFunc.h
│   └── core_cmInstr.h
├── Device/
│   ├── cm0dsasm.s
│   ├── EDK_CM0.h
│   ├── edk_driver.c
│   ├── edk_driver.h
│   ├── edk_api.c
│   ├── edk_api.h
│   └── retarget.c
├── vivado_project/           # Vivado project files
├── keil_project/             # Keil µVision project files
└── README.md                 # Project README file
```

## Usage

1. **Power on the Nexys A7 100T board** and ensure it is connected to your computer.
2. **Start the PONG game** by running the programmed logic on the FPGA and Cortex-M0.
3. **Control the paddles** using the connected buttons or switches.
4. **Enjoy the game** and challenge a friend!


## License

All files and resources in this project are subject to ARM's licensing terms and conditions. Please refer to the specific license files included in the repository or the ARM website for detailed information.

## Acknowledgements

- ARM Education for providing the Verilog files and educational resources.
- The open-source community for tools and support.

---

Feel free to reach out if you have any questions or need further assistance.

Happy gaming!
