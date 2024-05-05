# PRIORITY_ENCODER
# Aim:
To design and simulate Priority Encoder using vivado.

# Apparatus Required:
Pc with vivado software.

# Procedure
STEP:1 Start the Xilinx navigator, Select and Name the New project. 

STEP:2 Select the device family, device, package and speed. 

STEP:3 Select new source in the New Project and select Verilog Module as the Source type. 

STEP:4 Type the File Name and Click Next and then finish button. Type the code and save it. 

STEP:5 Select the Behavioral Simulation in the Source Window and click the check syntax. 

STEP:6 Click the simulation to simulate the program and give the inputs and verify the outputs as per the truth table. 

STEP:7 Select the Implementation in the Sources Window and select the required file in the Processes Window. 

STEP:8 Select Check Syntax from the Synthesize XST Process. Double Click in the FloorplanArea/IO/Logic-Post Synthesis process in the User Constraints process group. UCF(User constraint File) is obtained. 

STEP:9 In the Design Object List Window, enter the pin location for each pin in the Loc column Select save from the File menu. 

STEP:10 Double click on the Implement Design and double click on the Generate Programming File to create a bitstream of the design.(.v) file is converted into .bit file here. 

STEP:11 On the board, by giving required input, the LEDs starts to glow light, indicating the output.

![image](https://github.com/RESMIRNAIR/PRIORITY_ENCODER/assets/154305926/016b3b20-1d4d-48fd-9012-a2c725b822db)
# Truth Table
![image](https://github.com/RESMIRNAIR/PRIORITY_ENCODER/assets/154305926/3da43bab-6ee6-456f-858f-4553d3623f8c)
# Program:
module encoder(d,a,b,c);

input [7:0]d;

output a,b,c;

or(a,d[4],d[5],d[6],d[7]);

or(b,d[2],d[3],d[6],d[7]);

or(c,d[1],d[3],d[5],d[7]);

endmodule

# Output:
![image](https://github.com/navyasaik/PRIORITY_ENCODER/assets/165140258/fd4c0f07-3563-4210-a13d-d65bde00121e)
# Result:
Hence Priority Encoder is verified





