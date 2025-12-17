# SERIAL-IN-SERIAL-OUT-SHIFTREGISTER

**AIM:**

To implement  SISO Shift Register using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**SISO shift Register**

A Serial-In Serial-Out shift register is a sequential logic circuit that allows data to be shifted in and out one bit at a time in a serial manner. It consists of a cascade of flip-flops connected in series, forming a chain. The input data is applied to the first flip-flop in the chain, and as the clock pulses, the data propagates through the flip-flops, ultimately appearing at the output.

The logic circuit provided below demonstrates a serial-in serial-out (SISO) shift register. It comprises four D flip-flops that are interconnected in a sequential manner. These flip-flops operate synchronously with one another, as they all receive the same clock signal.

![image](https://github.com/naavaneetha/SERIAL-IN-SERIAL-OUT-SHIFTREGISTER/assets/154305477/e81c4072-37f9-46c6-8145-566764b74c3a)

Figure 01 4 Bit SISO Register

The synchronous nature of the flip-flops ensures that the shifting of data occurs in a coordinated manner. When the clock signal rises, the input data is sampled and stored in the first flip-flop. On subsequent clock pulses, the stored data propagates through the flip-flops, moving from one flip-flop to the next.
Each D flip-flop in the circuit has a Data (D) input, a Clock (CLK) input, and an output (Q). The D input represents the data to be loaded into the flip-flop, while the CLK input is connected to the common clock signal. The output (Q) of each flip-flop is connected to the D input of the next flip-flop, forming a cascade.

**Procedure**

1. Write the Verilog module for a SISO shift register with clock, reset, serial input, and serial output.

2. Use a clocked always block to shift data and load the serial input bit.

3. Reset the register to zero initially.

4. Create a testbench to apply clock and input signals.

5.Simulate and verify the output using the functional table.
/* write all the steps invloved */

**PROGRAM**
<img width="1920" height="1080" alt="SISO register program" src="https://github.com/user-attachments/assets/bbf4ddbb-e0de-4254-b9d7-a928d3ca25b2" />

/* Program for flipflops and verify its truth table in quartus using Verilog programming.

Developed by:S Tozer Theophilus RegisterNumber:25016814

*/

**RTL LOGIC FOR SISO Shift Register**
<img width="535" height="279" alt="SISO register RTL diagram" src="https://github.com/user-attachments/assets/402d55cf-2d93-419d-8496-6f35e14ddaea" />

**TIMING DIGRAMS FOR SISO Shift Register**
<img width="1920" height="1080" alt="SISO register waveform" src="https://github.com/user-attachments/assets/67741f55-9489-4c6c-a95e-dea25af7266f" />

**RESULTS**
The SISO shift register was implemented successfully in Verilog. Simulation results matched the functional table, confirming correct serial data shifting and output.
