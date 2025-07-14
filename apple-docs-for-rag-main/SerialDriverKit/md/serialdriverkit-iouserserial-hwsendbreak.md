

- SerialDriverKit
- IOUserSerial
-  HwSendBreak 

Instance Method

# HwSendBreak

Sends a linebreak command to the device.

DriverKit 19.0+

``` source
kern_return_t HwSendBreak(bool sendBreak);
```

## Parameters 

`sendBreak`  

A Boolean indicating whether to send a break command.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

Override this method and use it to set the break bit on the device.

## See Also

### Programming the Modem

HwGetModemStatus

Gets the current status of the modem from the hardware.

SetModemStatus

Sets the modem status to the specified values.

HwResetFIFO

Sends a command to reset the specified device queues.

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

