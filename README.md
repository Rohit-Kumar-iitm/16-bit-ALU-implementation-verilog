# Implementing a 16 bit ALU in Verilog HDL

- To build this ALU concepts from [Top-down design approach](https://www.techopedia.com/definition/9744/top-down-design) were used.

  - The top-level block/module is identified and then identification of the sub-blocks/modules necessary takes place to build the top-level block/module Main_module. 

  - Further subdivides are the sub-blocks/modules like adder, subtractor, multiplier and shifter until we come to leaf cells, which are the cells that cannot further be divided. 

  - Here the leaf cells are implemented using gate level design. 

  - The multiplier and shifter modules are designed using behavioral approach.

The Adder used is the Carry Look Ahead Adder of 16 bit wide bus length. 
The main top level module Main_module for 16 bit ALU calls the sub-module adder, subtractor, multiplier and shifter depending upon the select lines of the mux. 
Further the sub-modules are constructed by designing leaf cells cla_logic and PFAdder. 
These leaf cells are designed using gate level approach.
