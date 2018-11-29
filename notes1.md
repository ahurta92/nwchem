## Getting Started

NWChem consists of independent modules that perform the various functions of the code

Some examples of modules

input parser
SCF energy
SCF analytic gradient
DFT energy
Data is passed between modules ad saved for restart using a disk-resident database or dump file

 ## Input to NWChem is composed of commands, called directives, 
Directives: Defines Data/ Action on Data
Data: Basis set
    : Geometries
    : Filenames
Derectives processed in order presented in input file
Most directivces are specific to a particular module and define data to be used by module only 

A few directives affect all modules.  For example Total Electric Charge

## 2 Types of Directives

- Simple(one line of input,multiple feilds)
- Compound(multiple Simple directives)termintaed with END directive

## Information about Input

- input is free format and case is ignored (except actual data)
- Directives or blocks of module-specific directives can appear in any order
    - exception is the task directive which is used to invoke NWChem Module
    - all input for a given task must precede the TASK directive 
- This allows concatentation of multiple tasks in a single NWChem input file
- Most options have default values
    - user supply input for those with no default


## .nwchemrc

- Each user should have a .nwchemrc file to point to default data files, such as sets, psuedopotentials, and MD potentials
-  Contents of default.nwchemrc file based on the above iformation should be:
