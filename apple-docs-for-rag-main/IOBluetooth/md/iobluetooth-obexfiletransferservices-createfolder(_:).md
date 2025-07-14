

- IOBluetooth
- OBEXFileTransferServices
-  createFolder(\_:) 

Instance Method

# createFolder(\_:)

Create a folder on the remote target

macOS

``` source
func createFolder(_ inDirName: String!) -> OBEXError
```

## Parameters 

`inDirName`  

The name of the folder to be created

## Return Value

kOBEXSuccess, kOBEXSessionBusyError, or kOBEXBadArgumentError initially. Further results returned through the fileTransferServicesCreateFolderComplete delegate method if initially successful.

## Discussion

Equivalent to ‘mkdir dirName’.

