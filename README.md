# Test program for ODrive <-> Teensy PID feedback control
This program is a modification of the Arduino example program that comes with the Arduino-ODrive library. Like the original, it allows you to test the UART communication between the Teensy and the ODrive. However, I added the ability to test sending dual current commands which trigger a encoder reading response from the ODrive. These responses also give you the latency of the communication, measured from when the current command is sent to when the Teensy receives the response.

### Hardware requirements:
- ODrive 3.5
- Teensy 3.5
- UART connection between [RX1, TX1] on the Teensy and [GPIO2, GPIO1] on the ODrive
- Proper motor and encoder setup on the ODrive

### Software requirements:
- Flash this custom firmware onto the ODrive 3.5: https://github.com/Nate711/ODrive
- Configure the ODrive (https://docs.odriverobotics.com/)
