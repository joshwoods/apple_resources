

- IOBluetooth
- OBEXFileTransferServices
-  changeCurrentFolderForward(toPath:) 

Instance Method

# changeCurrentFolderForward(toPath:)

Change the remote path

macOS

``` source
func changeCurrentFolderForward(toPath inDirName: String!) -> OBEXError
```

## Parameters 

`inDirName`  

The name of the remote folder to be set as current

## Return Value

kOBEXSuccess, kOBEXSessionBusyError, or kOBEXBadArgumentError initially. Further results returned through the fileTransferServicesPathChangeComplete: delegate method if initially successful.

## Discussion

Equivalent to ‘cd dirName’.

