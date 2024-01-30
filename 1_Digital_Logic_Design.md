# Synchronous Reset and Asynchronous Reset
Synchronous reset: 
the reset has the same priority as the input signal, the output signal will be reseted at the clock edge.  
Applications:
1. Timing predictability: In high speed datapath or CPUs, synchronous reset avoids timing uncertainties since it's synchrounized with the clk signal. Ensure that the reset is timed precisely with other operations in CPUs.


asynchronous reset: 
the reset has the highest priority, the signal will be reseted when the reset is being set to high.
1. Low Power Design: An immediate reset to zero helps decrease power consumption.
2. Initialization: Sometimes before the clk starts, all the registers should be set to a known state.
3. Emergency: When emergency occurs, asynchronous reset shuts down the system immediately, safer.
