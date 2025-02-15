# Scripting_and_automation
This project automates the Vivado synthesis and implementation process using TCL scripts and Python. The main components of the project are:

## Tcl_scripting.ipynb

This Jupyter notebook automates the entire flow and generates results in a file named `results1.csv`. It likely uses Python to orchestrate the execution of TCL scripts and process the results.

## TCL Scripts

### tcl_add1.tcl

This script creates a project named "project3" and adds all the designs present in the "Modules" folder to the project. It streamlines the process of setting up a new Vivado project with multiple design files.

### tcl_run3.tcl

This script handles the synthesis of the code and stores the results. It automates the synthesis process, which is a crucial step in FPGA design.

## Design Files

The repository contains several Verilog design files that are used to test the automation tool. These designs include:

1. **dff**: A D flip-flop implementation
2. **multiply**: An 8-bit multiplier
3. **multiply_not_synth**: A large multiplier that is not synthesizable
4. **mux21**: A 2:1 multiplexer
5. **top_alubit.v**: Likely an ALU (Arithmetic Logic Unit) design
6. **top_koggestone_bit.v**: Possibly a Kogge-Stone adder implementation
7. **top_master_slave.v**: A master-slave flip-flop design
8. **top_moore.v**: A Moore state machine implementation
9. **top_knowels_bit.v**: Another bit-level design, possibly an adder variant
10. **top_lander_fisher_bit.v**: Likely a Lander-Fischer adder implementation
11. **top_mealy.v**: A Mealy state machine implementation
12. **top_ripplebit.v**: Probably a ripple-carry adder design

## Results

The `Results1.csv` file contains the synthesis results for each design. It provides information about the synthesizability and resource utilization of each design. If a row in the CSV file contains all zeros, it indicates that the corresponding design is not synthesizable.

This automation tool significantly streamlines the FPGA design process by:

1. Automatically creating projects and adding design files
2. Running synthesis and implementation steps
3. Generating reports and results in an easily analyzable format (CSV)

