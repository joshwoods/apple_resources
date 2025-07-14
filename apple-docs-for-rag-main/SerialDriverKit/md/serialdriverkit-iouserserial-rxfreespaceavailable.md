

- SerialDriverKit
- IOUserSerial
-  RxFreeSpaceAvailable 

Instance Method

# RxFreeSpaceAvailable

Notifies your driver that buffer space is available for your device’s data.

DriverKit 19.0+

``` source
void RxFreeSpaceAvailable();
```

## Discussion

Override this method and use it to read data asynchronously from the device’s serial port. When you finish reading the data, call the RxDataAvailable method to let the system know the data is ready.

## See Also

### Transmitting and Receiving Data

RxDataAvailable

Notifies the system that data from the device is now available.

TxDataAvailable

Notifies your driver that the system has data for you to transmit to the device.

TxFreeSpaceAvailable

Notifies the system that the device is ready to accept more data.

RxError

Reports errors that occurred when receiving data from the device.

