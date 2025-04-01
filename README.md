# TASK-2-VSDIAT-VLSI-SYSTEM-UART-LOOKBACK


# UART TX Project Documentation

## 1.1 Study the Existing Code
- I started by accessing the `uart_tx` project from the `VSDSquadron_FM` repository.
- After opening the Verilog code, I examined how the transmission process works. The main focus was on understanding how the data is transmitted bit by bit and how the control signals, such as the start and stop bits, are managed.

## 1.2 Design Documentation

### Block Diagram:
- I created the block diagram using **Draw.io** to illustrate the UART transmitter module. The diagram includes:
  - **Data Register**: Holds the data to be transmitted.
  - **UART TX Module**: Handles the actual transmission.
  - **Control Logic**: Manages the start and stop signals and synchronizes transmission.
  - 
![Screenshot (2496)](https://github.com/user-attachments/assets/3d908bcd-6b3d-4e96-ab78-db59357277c9)


### Circuit Diagram:
- I did not use a specific software tool for the circuit diagram but instead followed the general guidelines for pin connections. The FPGA's UART TX pin is connected to the receiving device's RX pin, and other connections were made based on the design requirements.

## 1.3 Implementation

### Hardware Setup:
- I physically connected the FPGA to the UART-compatible device following the connections from the circuit diagram. The setup was simple and involved using jumper wires to connect the relevant pins.

### Synthesize and Program the FPGA:
- For the synthesis and programming, I used **Xilinx Vivado**. The Verilog code was synthesized into a bitstream, and then I programmed the FPGA using Vivado's built-in programming tool.

## 1.4 Testing and Verification

### Connection to Receiving Device:
- To test the UART transmission, I connected the FPGA to a PC using a **USB-to-UART converter**.

### Software for Testing (Serial Terminal):
- I used **Tera Term** as the serial terminal software to monitor the data transmitted by the FPGA. The baud rate and other serial parameters were configured, and I confirmed that the data sent from the FPGA was correctly displayed on the terminal.

### Testing Results:
- During testing, I observed that the data was transmitted correctly and consistently, matching the expected output based on the configuration.

## 1.5 Documentation

### Block and Circuit Diagrams:
- The block diagram created with **Draw.io** is included in the documentation.
- I also described the circuit setup in detail, noting the key connections between the FPGA and the receiving device.

### Code Walkthrough:
- The Verilog code was reviewed and explained, highlighting the main components of the transmission logic and their interactions.

### Testing Outcomes:
- I documented that the transmitted data appeared correctly on the serial terminal in **Tera Term**, confirming successful transmission.

### Video Demonstration:
- The first time I performed the task, I successfully transmitted data and observed it in the serial terminal, but unfortunately, I did not record the video at that point.
- On the second attempt, I tried to record the video, but due to technical issues with my PC, the video did not work as expected. Despite this, the UART transmission was verified and tested successfully.



But I have the image of the led glowing by vm terminal





![20250327_220925](https://github.com/user-attachments/assets/0c7962e5-95d4-42f5-9162-465b7284bf01)


