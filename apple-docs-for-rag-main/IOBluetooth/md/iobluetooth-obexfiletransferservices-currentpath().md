

- IOBluetooth
- OBEXFileTransferServices
-  currentPath() 

Instance Method

# currentPath()

Get the remote current directory path during an FTP session

macOS

``` source
func currentPath() -> String!
```

## Return Value

The current path being browsed over FTP

## Discussion

This path is changed with each path-specific command called on OBEXFileTransferServices.

