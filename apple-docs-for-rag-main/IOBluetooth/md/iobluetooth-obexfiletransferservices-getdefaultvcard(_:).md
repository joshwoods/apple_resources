

- IOBluetooth
- OBEXFileTransferServices
-  getDefaultVCard(\_:) 

Instance Method

# getDefaultVCard(\_:)

Get the remote default VCard, if it is supported

macOS

``` source
func getDefaultVCard(_ inLocalPathAndName: String!) -> OBEXError
```

## Parameters 

`inLocalPathAndName`  

The path and name of where the received file will go

## Return Value

kOBEXSuccess, kOBEXSessionBusyError, or kOBEXBadArgumentError initially. Further results returned through the fileTransferServicesGetComplete: and fileTransferServicesGetProgress: delegate methods if initially successful.

## Discussion

Some devices such as cellphones and computers support default VCards

