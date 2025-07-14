

- SerialDriverKit
- IOUserSerial
-  SetModemStatus 

Instance Method

# SetModemStatus

Sets the modem status to the specified values.

DriverKit 19.0+

``` source
kern_return_t SetModemStatus(bool cts, bool dsr, bool ri, bool dcd);
```

## Parameters 

`cts`  

A Boolean value indicating the state of the clear-to-send bit. Specify `YES` to set the bit or `NO` to clear it.

`dsr`  

A Boolean value indicating the state of the data-set-ready bit. Specify `YES` to set the bit or `NO` to clear it.

`ri`  

A Boolean value indicating the state of the ring-indicator bit. Specify `YES` to set the bit or `NO` to clear it.

`dcd`  

A Boolean value indicating the state of the data-carrier-detect bit. Specify `YES` to set the bit or `NO` to clear it.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

Call this method to report the state of the device to the system.

## See Also

### Programming the Modem

HwGetModemStatus

Gets the current status of the modem from the hardware.

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

