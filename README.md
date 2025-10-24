# treadmill-controller

Repository for everything related to the (large) treadmill controller and the development of a replacement.


There is now a treadmill controller (V1!), seen in TreadmillController.ino, for the Arduino MEGA 2560. This code is loosely based on the code in the BEP-project, in the sense that we also write over serial1, and we used their lookup-table for the speed controls to the treadmill. The code now also has a serialmonitor if you connect a pc. We suspect this won't generate problems if there's no computer connected to the arduino.

Changes in the arduino diagram with respect to the arduino diagram in the BEP-project:
- Connect the RX to RX and TX to TX, instead of RX's to TX's
- In the report, pin 5 and 22 are connected, however it should be pin 5 with pin 7

For setup: the treadmill's controller (the white one) is still used here, it's controls are being bypassed by the arduino code in this repository.