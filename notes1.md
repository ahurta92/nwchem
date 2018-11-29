## Getting Started

NWChem consists of independent modules that perform the various functions of the code

Some examples of modules

input parser
SCF energy
SCF analytic gradient
DFT energy
Data is passed between modules ad saved for restart using a disk-resident database or dump file

2. Input to NWChem is composed of commands, called directives, 
Directives: Defines Data/ Action on Data
Data: Basis set
    : Geometries
    : Filenames
Derectives processed in order presented in input file
Most directivces are specific to a particular module and define data to be used by module only 

A few directives affect all modules.  For example Total Electric Charge

2 Types of Directives

Siple(one line of input,multiple feilds)
Compound(multiple Simple directives)termintaed with END directive

## Information about Input
 
- input is free format and case is ignored (except actual data)
- Directives or blocks of module-specific directives can appear in any order
    - exception is the task directive

