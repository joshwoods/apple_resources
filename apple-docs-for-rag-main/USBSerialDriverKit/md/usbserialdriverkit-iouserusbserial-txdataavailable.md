

- USBSerialDriverKit
- IOUserUSBSerial
-  TxDataAvailable 

Instance Method

# TxDataAvailable

Notifies your driver that the system has data for you to transmit to the device.

DriverKit 19.0+

``` source
void TxDataAvailable();
```

## Discussion

The default implementation of this method initiates an asynchronous operation to transmit the buffered data to the device.

## See Also

### Transmitting and Receiving Data

handleRxPacket

Processes the data received from the USB device.

RxFreeSpaceAvailable

Notifies your driver that buffer space is available for your device’s data.

handleInterruptPacket

Processes an interrupt packet that originated from the device.

