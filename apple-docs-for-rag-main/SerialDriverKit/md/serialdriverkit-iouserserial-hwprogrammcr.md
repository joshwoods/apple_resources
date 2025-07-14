

- SerialDriverKit
- IOUserSerial
-  HwProgramMCR 

Instance Method

# HwProgramMCR

Configure the setings for the device’s modem control register (MCR).

DriverKit 19.0+

``` source
kern_return_t HwProgramMCR(bool dtr, bool rts);
```

## Parameters 

`dtr`  

A Boolean value indicating whether to set or clear the data-terminal-ready bit. If the value is `YES`, set the bit; otherwise, clear it.

`rts`  

A Boolean value indicating whether to set or clear the request-to-send bit. If the value is `YES`, set the bit; otherwise, clear it.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

Override this method and use it to program your hardware with the specified information.

## See Also

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

HwProgramUART

Configure the settings for the device’s universal asynchronous receiver/transmitter (UART).

Hardware Constants

Configure your device with the appropriate parity and flow-control options.

