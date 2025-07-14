

- SerialDriverKit
- IOUserSerial
-  HwProgramLatencyTimer 

Instance Method

# HwProgramLatencyTimer

Sets the amount of time to wait before sending the current buffer to the device.

DriverKit 19.0+

``` source
kern_return_t HwProgramLatencyTimer(uint32_t latency);
```

## Parameters 

`latency`  

The number of milliseconds for the device to wait before sending a partial buffer to the host.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

Override this method and use it to configure a latency timer for the device. Rather than sending buffers only when they’re full, the latency timer ensures that the hardware sends any accumulated data at the specified interval.

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

HwProgramMCR

Configure the setings for the device’s modem control register (MCR).

HwProgramUART

Configure the settings for the device’s universal asynchronous receiver/transmitter (UART).

Hardware Constants

Configure your device with the appropriate parity and flow-control options.

