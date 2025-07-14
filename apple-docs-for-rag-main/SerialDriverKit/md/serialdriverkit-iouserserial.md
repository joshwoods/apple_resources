

- SerialDriverKit
-  IOUserSerial 

Class

# IOUserSerial

The class for building a service that communicates using a serial connection.

DriverKit 19.0+

``` source
class IOUserSerial;
```

## Overview

Subclass `IOUserSerial` and use it to implement a service for communicating with serial devices. This class automatically manages the buffers used to store incoming and outgoing data. You are responsible for configuring your hardware, and for reading and writing data at appropriate times. This class supports configuration through standard modem commands or using universal asynchronous receiver/transmitter (UART) hardware.

If your driver communicates with your device over USB, subclass IOUserUSBSerial (in the USBSerialDriverKit framework) instead of this class.

## Topics

### Configuring the Service

init

Handles the basic initialization of the service.

Start

Starts the current service and associates it with the specified provider.

Stop

Stops the service associated with the specified provider.

free

Performs any final cleanup for the service.

initWith

Initializes the private data structures associated with this class.

### Activating and Deactivating the Service

HwActivate

Opens the communication channel to the device.

HwDeactivate

Closes the communication channel to the device.

### Configuring the Serial Data Queues

ConnectQueues

Creates and configures the buffers that store the data moving to and from the device.

DisconnectQueues

Releases the buffers that manage data moving to and from the device.

### Programming the Modem

HwGetModemStatus

Gets the current status of the modem from the hardware.

SetModemStatus

Sets the modem status to the specified values.

HwResetFIFO

Sends a command to reset the specified device queues.

HwSendBreak

Sends a linebreak command to the device.

HwProgramBaudRate

Sets the communication baud rate to the specified value.

HwProgramLatencyTimer

Sets the amount of time to wait before sending the current buffer to the device.

HwProgramMCR

Configure the setings for the device’s modem control register (MCR).

HwProgramUART

Configure the settings for the device’s universal asynchronous receiver/transmitter (UART).

Hardware Constants

Configure your device with the appropriate parity and flow-control options.

### Transmitting and Receiving Data

RxDataAvailable

Notifies the system that data from the device is now available.

RxFreeSpaceAvailable

Notifies your driver that buffer space is available for your device’s data.

TxDataAvailable

Notifies your driver that the system has data for you to transmit to the device.

TxFreeSpaceAvailable

Notifies the system that the device is ready to accept more data.

RxError

Reports errors that occurred when receiving data from the device.

### Instance Methods

HwProgramFlowControl

## See Also

### Serial Interface

com.apple.developer.driverkit.family.serial

A Boolean value that indicates whether to match the driver against devices with serial communication interfaces.

