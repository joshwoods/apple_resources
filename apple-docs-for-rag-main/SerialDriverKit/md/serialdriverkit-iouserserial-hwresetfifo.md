

- SerialDriverKit
- IOUserSerial
-  HwResetFIFO 

Instance Method

# HwResetFIFO

Sends a command to reset the specified device queues.

DriverKit 19.0+

``` source
kern_return_t HwResetFIFO(bool tx, bool rx);
```

## Parameters 

`tx`  

If `YES`, reset the queue you use to transmit data; otherwise, don’t reset the queue.

`rx`  

If `YES`, reset the queue you use to receive data; otherwise, don’t reset the queue.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

Override this method and use it to reset your device.

## See Also

### Programming the Modem

HwGetModemStatus

Gets the current status of the modem from the hardware.

SetModemStatus

Sets the modem status to the specified values.

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

