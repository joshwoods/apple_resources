

- SerialDriverKit
- IOUserSerial
-  TxDataAvailable 

Instance Method

# TxDataAvailable

Notifies your driver that the system has data for you to transmit to the device.

DriverKit 19.0+

``` source
void TxDataAvailable();
```

## Discussion

The system calls this method to let you know that there is buffered data ready for you to transmit to the device. The default implementation of this method does nothing. Override it and use your implementation to transfer that data to your hardware.

## See Also

### Transmitting and Receiving Data

RxDataAvailable

Notifies the system that data from the device is now available.

RxFreeSpaceAvailable

Notifies your driver that buffer space is available for your device’s data.

TxFreeSpaceAvailable

Notifies the system that the device is ready to accept more data.

RxError

Reports errors that occurred when receiving data from the device.

