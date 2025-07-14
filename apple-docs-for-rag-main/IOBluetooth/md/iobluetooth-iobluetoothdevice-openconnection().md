

- IOBluetooth
- IOBluetoothDevice
-  openConnection() 

Instance Method

# openConnection()

Create a baseband connection to the device.

macOS

``` source
func openConnection() -> IOReturn
```

## Return Value

Returns kIOReturnSuccess if the connection was successfully created.

## Discussion

This method is synchronous and will not return until either a connection has been established or the create connection has failed (perhaps timed out). This method does the same thing as calling -openConnection: with a nil target. This call with proceed without authentication required, and using the default page timeout value. If authentication or a non-default page timeout is required the method -openConnection:withPageTimeout:authenticationRequired: should be used instead.

As of OS X 10.7, this method will no longer mask out “Connection Exists” ‘errors’ with a success result code; your code must account for the cases where the baseband connection is already open.

