

- IOBluetooth
- OBEXFileTransferServices
-  removeItem(\_:) 

Instance Method

# removeItem(\_:)

Remove a remote item.

macOS

``` source
func removeItem(_ inItemName: String!) -> OBEXError
```

## Parameters 

`inItemName`  

The name of the remote item to be removed

## Return Value

kOBEXSuccess, kOBEXSessionBusyError, or kOBEXBadArgumentError initially. Further results returned through the fileTransferServicesRemoveItemComplete: delegate method if initially successful.

## Discussion

Not supported for use on Apple computer targets

