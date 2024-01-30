## Synchronous Reset and Asynchronous Reset
Synchronous reset:   
The reset has the same priority as the input signal, the output signal will be reseted at the clock edge.  
Benefits:
1. Timing predictability: In high speed datapath or CPUs, synchronous reset avoids timing uncertainties since it's synchrounized with the clk signal. Ensure that the reset is timed precisely with other operations in CPUs.


Asynchronous reset:   
The reset has the highest priority, the signal will be reseted when the reset is being set to high.  
Benefits:  
1. Low Power Design: An immediate reset to zero helps decrease power consumption.
2. Initialization: Sometimes before the clk starts, all the registers should be set to a known state.
3. Emergency: When emergency occurs, asynchronous reset shuts down the system immediately, safer.

## Mealy and Moore finite state machine
Mealy: The output depends on the present states and the input.  
Moore: The output depends on the present states only.  
When designing a CPU, we may prefer Moore finite state machine since the CPU needs to know the type of instructions, the data in the instructions.
