An automated Arduino fish feeder project that coordinates a 7-segment display with a servo motor. The system counts down or displays patterns across digital output pins (pins 2 through 8) to indicate status before triggering the servo motor (attached to pin 9) to dispense food.

### Features

* **Status Display:** Uses a 7-segment display connected to pins 2–8 to show custom sequences or countdowns during operation.
* **Automated Dispensing:** Utilizes a standard servo motor to open and close the food compartment.
* **Simple & Reliable:** Built using basic Arduino digital I/O control and the standard `Servo` library without requiring complex external modules.
