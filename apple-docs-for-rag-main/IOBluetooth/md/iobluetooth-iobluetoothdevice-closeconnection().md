

- IOBluetooth
- IOBluetoothDevice
-  closeConnection() 

Instance Method

# closeConnection()

Close down the baseband connection to the device.

macOS

``` source
func closeConnection() -> IOReturn
```

## Return Value

Returns kIOReturnSuccess if the connection has successfully been closed.

## Discussion

This method is synchronous and will not return until the connection has been closed (or the command failed). In the future this API will be changed to allow asynchronous operation.

