

- IOBluetooth
- IOBluetoothL2CAPChannel
-  close() 

Instance Method

# close()

Initiates the close process on an open L2CAP channel.

macOS

``` source
func close() -> IOReturn
```

## Return Value

Returns kIOReturnSuccess on success.

## Discussion

This method may only be called by the client that opened the channel in the first place. In the future asynchronous and synchronous versions will be provided that let the client know when the close process has been finished.

