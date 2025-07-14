

- SerialDriverKit
- IOUserSerial
-  HwProgramUART 

Instance Method

# HwProgramUART

Configure the settings for the device’s universal asynchronous receiver/transmitter (UART).

DriverKit 19.0+

``` source
kern_return_t HwProgramUART(uint32_t baudRate, uint8_t nDataBits, uint8_t nHalfStopBits, uint8_t parity);
```

## Parameters 

`baudRate`  

The baud rate requested by the system.

`nDataBits`  

The number of data bits to transmit.

`nHalfStopBits`  

The number of half stop bits. For example, specify `3` to generate `1.5` stop bits.

`parity`  

The parity setting to use during communication. For a list of possible values, see Parity Options.

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

HwProgramMCR

Configure the setings for the device’s modem control register (MCR).

Hardware Constants

Configure your device with the appropriate parity and flow-control options.

