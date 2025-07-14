

- IOBluetooth
- OBEXFileTransferServices
-  connectToFTPService() 

Instance Method

# connectToFTPService()

Connect to a remote device for FTP operations

macOS

``` source
func connectToFTPService() -> OBEXError
```

## Return Value

kOBEXSuccess, kOBEXSessionBusyError, or kOBEXSessionAlreadyConnectedError, kOBEXNoResourcesError initially. Further results returned through the fileTransferServicesConnectionComplete: delegate method if initially successful.

## Discussion

If the OBEXSession given to OBEXFileTransferServices on creation is not connected it can be manually connected through this method.

