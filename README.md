# TASK-2-VSDIAT-VLSI-SYSTEM-UART-LOOKBACK

# UART Loopback System – Block Diagram Design

### 1. Introduction
I worked on a UART loopback system to check if data sent from a device is correctly received back by the same device. The system includes a **FPGA**, a **UART Transmitter**, a **UART Receiver**, and a **Serial Terminal**. I created a block diagram to show how these components interact and how data flows between them.

### 2. Objective
The goal was to design a block diagram that shows:
- How the different parts of the UART loopback system work together.
- How data moves through the system from one component to another.

### 3. Components Involved
The system has these main components:
- **FPGA (or Microcontroller):** This is the main controller that handles everything, including the loopback process.
- **UART Transmitter:** It sends data from the FPGA to an external device, like a serial terminal.
- **UART Receiver:** It receives the data sent back from the serial terminal to the FPGA.
- **Serial Terminal (Software):** This is a program on the computer that communicates with the FPGA through UART.

### 4. Steps to Create the Block Diagram

#### 4.1 Identifying Key Components:
I started by identifying the key components involved in the system: FPGA, UART Transmitter, UART Receiver, and Serial Terminal.

#### 4.2 Defining Inputs and Outputs:
Then, I figured out what the inputs and outputs would be:
- **Inputs:** Data coming from the serial terminal to the FPGA.
- **Outputs:** Data sent back from the FPGA to the serial terminal.

#### 4.3 Choosing a Tool:
I used **Draw.io** (a free online tool) to create the block diagram. It's simple and provides all the shapes I needed to represent the components.

#### 4.4 Creating the Blocks:
I made blocks for each of the components and labeled them. Each block represents a part of the system, like the FPGA or the UART Transmitter.

#### 4.5 Connecting the Blocks:
I drew arrows between the blocks to show how the data moves:
- From the **Serial Terminal** to the **UART Transmitter** (FPGA).
- From the **UART Receiver** back to the **FPGA**.

#### 4.6 Labeling the Connections:
I labeled the connections to make it clear:
- **Data Out**: From FPGA to UART Transmitter.
- **Data In**: From UART Receiver to FPGA.
- I also labeled the data lines as **TX Data** and **RX Data**.

### 5. Example Block Diagram Explanation

The block diagram looks something like this:

Serial Terminal → UART Transmitter (FPGA) → UART Receiver (FPGA) → Serial Terminal.


- **Data Flow:** The **Serial Terminal** sends data to the FPGA, which then transmits it via the **UART Transmitter**. The **UART Receiver** receives the data back, which goes back to the **Serial Terminal**.

### 6. Tools Used
I used **Draw.io** to create the block diagram. It's an easy-to-use, free tool that I found perfect for this task. Other tools like **Lucidchart** or **Microsoft Visio** could also work, but I found **Draw.io** to be the most convenient.

### 7. Conclusion

By creating the block diagram, I was able to better understand how the components of the UART loopback system work together. It was helpful to visualize the data flow and make sure everything is connected correctly. Using **Draw.io** made the process easier, and now I have a clear diagram showing how the system operates.


### How I know : 

I reffered CHATGPT and Youtube for edocumenting such this this
