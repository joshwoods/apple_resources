

- USBSerialDriverKit
- IOUserUSBSerial
-  handleInterruptPacket 

Instance Method

# handleInterruptPacket

Processes an interrupt packet that originated from the device.

DriverKit 19.0+

``` source
void handleInterruptPacket(const uint8_t * packet, uint32_t size);
```

## Parameters 

`packet`  

A buffer containing the interrupt-related data.

`size`  

The number of bytes in the `packet` buffer.

## Discussion

Override this method if you want to process interrupt packets sent by the device. The default implementation of this method does nothing.

## See Also

### Transmitting and Receiving Data

handleRxPacket

Processes the data received from the USB device.

RxFreeSpaceAvailable

Notifies your driver that buffer space is available for your device’s data.

TxDataAvailable

Notifies your driver that the system has data for you to transmit to the device.

