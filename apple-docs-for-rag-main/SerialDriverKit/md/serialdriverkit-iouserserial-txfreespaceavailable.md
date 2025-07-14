

- SerialDriverKit
- IOUserSerial
-  TxFreeSpaceAvailable 

Instance Method

# TxFreeSpaceAvailable

Notifies the system that the device is ready to accept more data.

DriverKit 19.0+

``` source
void TxFreeSpaceAvailable();
```

## Discussion

Call this method after freeing up space in the memory buffer you use to transmit data. When more data is available, the system responds by adding that data to the buffer and calling the TxDataAvailable method.

## See Also

### Transmitting and Receiving Data

RxDataAvailable

Notifies the system that data from the device is now available.

RxFreeSpaceAvailable

Notifies your driver that buffer space is available for your device’s data.

TxDataAvailable

Notifies your driver that the system has data for you to transmit to the device.

RxError

Reports errors that occurred when receiving data from the device.

