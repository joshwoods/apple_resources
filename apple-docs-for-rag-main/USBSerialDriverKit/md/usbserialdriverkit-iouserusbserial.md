

- USBSerialDriverKit
-  IOUserUSBSerial 

Class

# IOUserUSBSerial

A service that manages a serial connection to a USB device.

DriverKit 19.0+

``` source
class IOUserUSBSerial;
```

## Overview

Subclass `IOUserUSBSerial` to implement a driver that communicates with a USB device serially. After matching your driver to the appropriate device, the system starts your driver and calls its HwActivate method, which you use to open and configure the communications channel for your device. Configure other hardware-related settings by overriding the appropriate methods defined in the IOUserSerial parent class.

This class automatically manages the serial communications with the device, buffering data received from it. The class creates the buffers for holding data, and initiates asynchronous operations to the USB device to transmit and receive data. Use the methods of this class to modify the data, as needed.

## Topics

### Configuring the Service

init

Handles the basic initialization of the service.

Start

Starts the service for the specified provider.

Stop

Stops the service that matches the specified provider.

free

Performs any final cleanup for the service.

initWith

Initializes the private data structures associated with this class.

### Activating and Deactivating the Service

HwActivate

Opens the communication channel to the device.

HwDeactivate

Closes the communication channel to the device.

### Transmitting and Receiving Data

handleRxPacket

Processes the data received from the USB device.

RxFreeSpaceAvailable

Notifies your driver that buffer space is available for your device’s data.

TxDataAvailable

Notifies your driver that the system has data for you to transmit to the device.

handleInterruptPacket

Processes an interrupt packet that originated from the device.

### Configuring the Serial Data Queues

ConnectQueues

Creates and configures the buffers that store the data moving to and from the device.

DisconnectQueues

Releases the buffers that manage data moving to and from the device.

## See Also

### Serial USB Interface

com.apple.developer.driverkit.family.serial

A Boolean value that indicates whether to match the driver against devices with serial communication interfaces.

