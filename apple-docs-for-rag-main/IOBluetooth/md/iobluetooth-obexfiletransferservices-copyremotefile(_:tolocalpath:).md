

- IOBluetooth
- OBEXFileTransferServices
-  copyRemoteFile(\_:toLocalPath:) 

Instance Method

# copyRemoteFile(\_:toLocalPath:)

Copy a remote file to a local path

macOS

``` source
func copyRemoteFile(
    _ inRemoteFileName: String!,
    toLocalPath inLocalPathAndName: String!
) -> OBEXError
```

## Parameters 

`inRemoteFileName`  

The name of the remote file to get

`inLocalPathAndName`  

The path and name of where the received file will go

## Return Value

kOBEXSuccess, kOBEXSessionBusyError, or kOBEXBadArgumentError. initially. Further results returned through the fileTransferServicesGetComplete: and fileTransferServicesGetProgress: delegate methods if initially successful.

## Discussion

Equivalent to ‘cp remotePath/remoteFileName localPathAndName’.

