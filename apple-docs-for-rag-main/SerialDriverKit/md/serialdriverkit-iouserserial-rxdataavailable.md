

- SerialDriverKit
- IOUserSerial
-  RxDataAvailable 

Instance Method

# RxDataAvailable

Notifies the system that data from the device is now available.

DriverKit 19.0+

``` source
void RxDataAvailable();
```

## Discussion

After receiving data from the device and placing it in your data buffer, call this method to let the system know that the data is available.

## See Also

### Transmitting and Receiving Data

RxFreeSpaceAvailable

Notifies your driver that buffer space is available for your device’s data.

TxDataAvailable

Notifies your driver that the system has data for you to transmit to the device.

TxFreeSpaceAvailable

Notifies the system that the device is ready to accept more data.

RxError

Reports errors that occurred when receiving data from the device.

