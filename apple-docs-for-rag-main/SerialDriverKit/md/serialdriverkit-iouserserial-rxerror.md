

- SerialDriverKit
- IOUserSerial
-  RxError 

Instance Method

# RxError

Reports errors that occurred when receiving data from the device.

DriverKit 19.0+

``` source
kern_return_t RxError(bool overrun, bool gotBreak, bool framingError, bool parityError);
```

## Parameters 

`overrun`  

A Boolean value indicating whether a buffer overrun error occurred.

`gotBreak`  

A Boolean value indicating whether a break error occurred.

`framingError`  

A Boolean value indicating whether a framing error occurred.

`parityError`  

A Boolean value indicating whether a parity error occurred.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

Call this method when you encounter an error getting data from the device.

## See Also

### Transmitting and Receiving Data

RxDataAvailable

Notifies the system that data from the device is now available.

RxFreeSpaceAvailable

Notifies your driver that buffer space is available for your device’s data.

TxDataAvailable

Notifies your driver that the system has data for you to transmit to the device.

TxFreeSpaceAvailable

Notifies the system that the device is ready to accept more data.

