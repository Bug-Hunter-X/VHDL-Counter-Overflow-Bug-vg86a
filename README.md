# VHDL Counter with Overflow Bug

This repository demonstrates a common but subtle bug in VHDL: an integer counter that lacks overflow protection.  The `counter.vhdl` file contains the buggy code. When the counter reaches its maximum value (15), it will wrap around to 0 instead of stopping or signaling an error. This can lead to incorrect behavior in systems relying on the counter's value.

The solution, provided in `counter_fixed.vhdl`, adds a check to prevent overflow, handling the maximum value appropriately. This example highlights the importance of considering potential overflow scenarios when designing VHDL code for hardware.