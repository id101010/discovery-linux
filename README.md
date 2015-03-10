BFH stm32f4 discovery linuxsupport
============================

## Synopsis

The following project consists of a minimal setup for the STM32 discovery board. The makefile should be easily adaptable to your needs. 

## Motivation

We'd like to enable linux enthusiastic students of the bern university of applied sciences to work with their beloved operating system without setting up a virtual machine just to run *atollic true studio*. ;)

## Installation and required packages

You'll need the following packages installed on your system: 

        arm-none-eabi-binutils
        arm-none-eabi-gcc
        arm-none-eabi-gdb
        arm-none-eabi-newlib
        stlink
        make

The package names are taken from the arch linux community repository, hence they may differ on your linux distribution.

## Instructions

####first steps
   
- Clone the repository.
- Install the required software packages.
- Plug in your discovery board.
- Don't forget to add yourself to the group 'dialout' by invoking "gpasswd -a ${USER} dialout"
    
#### using make

- Build software: make all
- Debug software: make debug
- flash software: make flash
- start/stop st-util deamon: make start/stop

#### eclipse support

If you want to use eclipse instead of pure makefiles you are free to do so and we are happy to support you with that:

- Checkout the readme in the eclipse directory for instructions on how to install and configure eclipse correctly.
- Import the example project into eclipse as "existing project" and have fun :)

## Contributors

- t-moe
- id101010

## Links

- http://www.st.com/web/en/catalog/tools/FM116/SC959/SS1532/PF250863?sc=stm32-discovery

## Additional Tags

stm32, stm-discovery, discovery board, bfh ti, berner fachhochschule für technik und informatik, linux
