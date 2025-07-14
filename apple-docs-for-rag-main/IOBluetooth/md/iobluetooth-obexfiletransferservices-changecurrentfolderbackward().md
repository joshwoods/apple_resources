

- IOBluetooth
- OBEXFileTransferServices
-  changeCurrentFolderBackward() 

Instance Method

# changeCurrentFolderBackward()

Change to the directory above the current level if not at the root

macOS

``` source
func changeCurrentFolderBackward() -> OBEXError
```

## Return Value

kOBEXSuccess or kOBEXSessionBusyError initially. Further results returned through the fileTransferServicesPathChangeComplete: delegate method if initially successful.

## Discussion

Equivalent to ‘cd ..’ only if remote path is not already at root.

