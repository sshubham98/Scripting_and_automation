# FPGA Design Automation Framework

## Project Overview
This project automates the Vivado synthesis and implementation process using TCL scripts and Python. It streamlines FPGA design workflows by automating project creation, synthesis, and result reporting.

## Key Components

### 1. Tcl_scripting.ipynb
A Jupyter notebook that orchestrates the entire automation flow:
- Executes TCL scripts
- Processes synthesis results
- Generates the final `1.results.csv` file

### 2. TCL Scripts
#### tcl_add1.tcl
- Creates a Vivado project named "project3"
- Adds all designs from the "Modules" folder to the project

#### tcl_run3.tcl
- Handles synthesis of the designs
- Stores synthesis results

### 3. Design Files
The repository includes various Verilog design files for testing the automation tool:

1. `multiply_not_synth.v`: A large, non-synthesizable multiplier (for testing error handling)
2. `top_master_slave.v`: Master-slave flip-flop implementation
3. `top_mux21.v`: 2:1 multiplexer design
4. `top_alubit.v`: ALU (Arithmetic Logic Unit) design
5. `top_mealy.v`: Mealy state machine implementation
6. `top_ripplebit.v`: Ripple-carry adder design
7. `top_binary_decoder.v`: Binary decoder implementation
8. `top_moore.v`: Moore state machine implementation
9. `top_synchronous_counter.v`: Synchronous counter design
10. `top_dff.v`: D flip-flop implementation
11. `top_multiply.v`: 8-bit multiplier design
12. `top_universal_shift_reg.v`: Universal shift register implementation

### 4. Results
The `Results1.csv` file contains synthesis results for each design, including:
- Resource utilization (LUTs, FFs, DSPs, etc.)
- Power consumption
- Timing information
- Synthesizability flag (designs with all zeros are not synthesizable)

## Benefits of Automation
1. Batch processing of multiple designs
2. Consistent project setup and synthesis flow
3. Automated report generation in CSV format for easy analysis
4. Quick identification of non-synthesizable designs
5. Significant time savings in the FPGA design process
