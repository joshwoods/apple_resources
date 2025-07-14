

- IOBluetooth
- OBEXFileTransferServices
-  withOBEXSession(\_:) 

Type Method

# withOBEXSession(\_:)

Create a new OBEXFileTransferServices object

macOS

``` source
class func withOBEXSession(_ inOBEXSession: IOBluetoothOBEXSession!) -> Self!
```

## Parameters 

`inOBEXSession`  

A valid IOBluetoothOBEXSession

## Return Value

A newly created OBEXFileTransferServices object on success, nil on failure

## Discussion

This object must be constructed with a valid IOBluetoothOBEXSession. The given IOBluetoothOBEXSession does not need to be connected to the remote server. This module can be manually connected through the connect() method.

