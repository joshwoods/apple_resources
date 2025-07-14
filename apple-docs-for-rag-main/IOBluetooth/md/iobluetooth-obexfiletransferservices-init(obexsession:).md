

- IOBluetooth
- OBEXFileTransferServices
-  init(obexSession:) 

Initializer

# init(obexSession:)

Create a new OBEXFileTransferServices object

macOS

``` source
init!(obexSession inOBEXSession: IOBluetoothOBEXSession!)
```

## Parameters 

`inOBEXSession`  

A valid IOBluetoothOBEXSession

## Return Value

A newly created OBEXFileTransferServices object on success, nil on failure

## Discussion

This object must be constructed with a valid IOBluetoothOBEXSession. The given IOBluetoothOBEXSession does not need to be connected to the remote server. OBEXFileTransferServices can be manually connected through the provided connection methods.

