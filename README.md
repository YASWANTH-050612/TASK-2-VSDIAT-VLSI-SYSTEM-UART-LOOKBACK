# TASK-2-VSDIAT-VLSI-SYSTEM-UART-LOOKBACK

# UART Loopback Task Documentation

## Task Overview

In this task, I worked with the VSDSquadron FPGA Mini to implement and test a UART loopback functionality. The goal was to send data from the terminal to the FPGA and receive the same data back, confirming that the loopback feature working as expected but not recorded and  second time it didn't work

---

## 1. Study the Existing Code

- **Objective**: I started by accessing the `uart_loopback` project from the VSDSquadron_FM repository.
- **Action**: I carefully reviewed the Verilog code to understand how the loopback logic was implemented. It was important to see how the data was being transmitted and received in the system.

---


## 2. Implementation

### Setting up the Hardware:

I set up the hardware as per the circuit diagram. It was crucial to ensure that all connections were correctly made before moving forward with the flashing process.

### Flashing the FPGA:

Once the hardware setup was complete, I used the following commands to build and flash the code to the FPGA:


cd VSDSquadron_FM/uart_lookback
make clean
make build
sudo make flash


---

## 3. Documentation

I compiled all of the steps I followed into this report. This includes the following:

### Block Diagram

- When I created the block diagram, it helped me visualize how the entire UART loopback system would work. The diagram clearly shows how data flows from the terminal (my computer) to the FPGA, and how the FPGA processes and sends it back. I connected the **TX** (transmit) pin of the FPGA directly to the **RX** (receive) pin, which forms the core of the loopback. This configuration allows the data sent from the FPGA to be immediately received by it, completing the loop. I had to double-check the connections to make sure the loopback was set up correctly, as it was the foundation of the whole testing process. Without this clear layout, I wouldn't have been able to proceed smoothly with the hardware setup.

![Screenshot (2496)](https://github.com/user-attachments/assets/3d908bcd-6b3d-4e96-ab78-db59357277c9)


### Circuit Diagram

- The circuit diagram was essential for the hardware setup. It showed me exactly how to wire the FPGA’s **TX** and **RX** pins to the corresponding serial interface. Once I reviewed the circuit diagram, I was confident that the physical setup matched the logic outlined in the block diagram. I used this to double-check that all the wiring was correct before proceeding with the code upload. This step was crucial because if any connection was wrong, the loopback wouldn’t work, and I could face issues later during testing. The circuit diagram gave me a clear roadmap of the connections I needed to make, and it was a great reference during the physical setup.



### Explanations of the Code

- The Verilog code was designed to handle the UART communication—sending data from the terminal to the FPGA and back. Initially, I spent some time going through the code to make sure it was implemented correctly. I checked that the **TX** and **RX** pins on the FPGA were properly connected in the code so the data could be sent out and received back without issues. The key part of the code was ensuring that the FPGA knew when to send data and when to wait for incoming data on the **RX** pin. Additionally, I made sure the timing and synchronization in the code were correct, which is crucial for any UART communication to function reliably. After a few tweaks, I was able to make sure everything was in order before flashing the code to the FPGA. This was the trickiest part, but also the most rewarding once I confirmed everything worked.

### Test Results Showing the Loopback Functionality in Action

- When I finally tested the loopback, I felt a sense of accomplishment. I opened **PuTTY** and sent some test data from the terminal to the FPGA. After hitting send, I anxiously waited to see if the same data would come back to the terminal. When the exact data appeared on the terminal screen, I immediately knew that the loopback was working. The data sent from the terminal matched exactly with the data that came back from the FPGA, confirming that the loopback functionality was functioning as expected. This was the moment when everything came together: the block diagram, circuit diagram, and code all lined up, and the system worked perfectly. It was a big win, and I was excited to see everything in action!

---

## 4. Recording

- The demonstatration was not recorded at first attempt and because of some issues in my Laptop (PC) the Serial terminal as I used Putty is showing error on that  and there is a troble in the loading of systhesis of Verilog code ...
  


---

## 5. Conclusion

- The UART loopback test was a success! I was able to send data from the terminal to the FPGA and receive the exact same data back. This confirmed that the loopback functionality works as expected  at first attempt I did successfully but  not in other times  and forget to record a vedio
- 
- Overall, the project was a valuable learning experience. From reviewing the code, setting up the hardware, to finally testing the system, I gained a better understanding of UART communication and how to implement loopback functionality effectively.

- But because of some reasons it was not loading .......

- But I have the screenshot of the output as red colour led which we should do in the terminal.

![20250327_220925](https://github.com/user-attachments/assets/0c7962e5-95d4-42f5-9162-465b7284bf01)


  May be same work will be done again on Task - 3 .....
