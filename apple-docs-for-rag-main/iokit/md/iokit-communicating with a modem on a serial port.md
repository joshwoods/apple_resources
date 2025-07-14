

- IOKit
-  Communicating with a Modem on a Serial Port 

Sample Code

# Communicating with a Modem on a Serial Port

Find and connect to a modem attached to a serial port using IOKit.

Download

macOS 10.6+Xcode 11.2+

## Overview

This sample project creates a command-line program that uses IOKit to discover a modem on a serial port and to send and receive data. Run the program within Xcode and use the console to monitor the progress of the communication.

### Discover Attached Modems

IOKit provides a matching service for various types of I/O devices, including serial ports and modems. The sample code’s `findModems()` function uses `kIOSerialBSDServiceValue` to locate a serial device. Once located, the code identifies the type of serial device as a modem with `kIOSerialBSDModemType`.

The `findModems()` function returns an IOKit iterator that `getModemPath()` uses to locate the first available modem and obtain its formal BSD device path.

If the function fails to find a modem or can’t obtain the device, the program prematurely quits.

### Open the Serial Port and Initialize the Modem

After the `findModems` function finds the modem, `openSerialPort()` uses the low-level `open()` call to connect to the BSD file path discovered earlier. This function also captures the state of the serial port and saves it for later restoration.

This code allows the function to set up communication parameters such as baud rate, blocking characteristics, and handshaking lines.

If the call succeeds, it returns a BSD file descriptor. The `initalizeModem()` function then takes the file descriptor and sends the attention (`AT`) command to the modem using the low-level `write()` function. It then calls the `read()` function to obtain a response that confirms the modem is present.

### Close the Serial Port

The `closeSerialPort()` function takes the passed file descriptor and waits for all output to flush, then restores the serial port to its original state and closes the file descriptor.

This action terminates communication to the modem and concludes the use of the serial port.

