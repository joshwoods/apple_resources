

- IOBluetooth
- OBEXFileTransferServices
-  sendFile(\_:) 

Instance Method

# sendFile(\_:)

Put a local file to the remote target

macOS

``` source
func sendFile(_ inLocalPathAndName: String!) -> OBEXError
```

## Parameters 

`inLocalPathAndName`  

The name and path of the file to be sent an instance of OBEXFilePut.

## Return Value

kOBEXSuccess, kOBEXSessionBusyError, or kOBEXBadArgumentError initially. Further results returned through the fileTransferServicesSendComplete: and fileTransferServicesSendProgress: delegate methods if initially successful.

## Discussion

Equivalent to ‘mv inLocalFilePath remoteCurrentPath’.

