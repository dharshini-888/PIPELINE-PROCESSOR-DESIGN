# PIPELINE-PROCESSOR-DESIGN

company:CODTECH IT SOLUTIONS

name:Dharshini

Intern id:CTO4DF2111

Domain:VLSI

DURATION:4 WEEKS

Mentor:NEELA SANTOSH

DESCRIPTION OF THE TASK The task involves designing a 4-stage pipelined processor in Verilog that can perform basic instructions such as ADD, SUB, and LOAD. The design demonstrates instruction execution through the following stages of a pipeline:

Pipeline Stages Instruction Fetch (IF):

Fetches the instruction from the instruction memory. Updates the program counter (PC) to fetch the next instruction. Instruction Decode (ID):

Decodes the fetched instruction to identify the operation (opcode) and operands (registers or immediate values). Reads source operands from the register file. Execute (EX):

Performs arithmetic and logical operations using the ALU (Arithmetic Logic Unit). For LOAD instructions, calculates the effective memory address. Memory Access (MEM):

Accesses the data memory for LOAD/STORE instructions. Passes the results of arithmetic instructions for the next stage. Write Back (WB):

Writes the results back to the destination register for arithmetic or LOAD instructions. Key Components Program Counter (PC):

output Time=0 R3= 0 Time=15 R3= 0 Time=25 R3= 0 Time=35 R3= 0 Time=45 R3= 30 // 10 (R1) + 20 (R2) Output R3 = 30 after pipeline delay — result appears around the 5th cycle due to 5-stage pipeline latency.



Holds the address of the current instruction. Updates to point to the next instruction after each clock cycle. Instruction Memory:

Stores the instructions for execution. Register File:

A set of registers for storing operands and results. Two read ports and one write port for efficient operation. ALU (Arithmetic Logic Unit):

Performs arithmetic (ADD, SUB) and logical operations. Data Memory:

Used for LOAD/STORE instructions. Pipeline Registers:

Separates the stages of the pipeline to hold intermediate data and control signals.
