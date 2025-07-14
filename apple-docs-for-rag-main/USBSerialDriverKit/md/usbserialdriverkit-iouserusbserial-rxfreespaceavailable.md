

- USBSerialDriverKit
- IOUserUSBSerial
-  RxFreeSpaceAvailable 

Instance Method

# RxFreeSpaceAvailable

Notifies your driver that buffer space is available for your device’s data.

DriverKit 19.0+

``` source
void RxFreeSpaceAvailable();
```

## Discussion

The default implementation of this method initiates an asynchronous operation to read data from the USB device.

## See Also

### Transmitting and Receiving Data

handleRxPacket

Processes the data received from the USB device.

TxDataAvailable

Notifies your driver that the system has data for you to transmit to the device.

handleInterruptPacket

Processes an interrupt packet that originated from the device.

