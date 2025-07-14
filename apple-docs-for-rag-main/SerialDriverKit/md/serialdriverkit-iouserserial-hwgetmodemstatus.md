

- SerialDriverKit
- IOUserSerial
-  HwGetModemStatus 

Instance Method

# HwGetModemStatus

Gets the current status of the modem from the hardware.

DriverKit 19.0+

``` source
kern_return_t HwGetModemStatus(bool * cts, bool * dsr, bool * ri, bool * dcd);
```

## Parameters 

`cts`  

On return, a Boolean variable containing the state of the clear-to-send bit. Set this value to `YES` when the bit is set.

`dsr`  

On return, a Boolean variable containing the state of the data-set-ready bit. Set this value to `YES` when the bit is set.

`ri`  

On return, a Boolean variable containing the state of the ring-indicator bit. Set this value to `YES` when the bit is set.

`dcd`  

On return, a Boolean variable containing the state of the data-carrier-detect bit. Set this value to `YES` when the bit is set.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

Override this method and use it to retrieve the current modem status from your hardware. Set the values of each parameter to an appropriate value based on whether the indicated bit is set.

## See Also

### Programming the Modem

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

