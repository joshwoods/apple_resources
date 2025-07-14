

- IOBluetooth
- OBEXFileTransferServices
-  retrieveFolderListing() 

Instance Method

# retrieveFolderListing()

Get a remote directory listing

macOS

``` source
func retrieveFolderListing() -> OBEXError
```

## Return Value

kOBEXSuccess or kOBEXSessionBusyError initially. Further results returned through the fileTransferServicesRetrieveFolderListingComplete: delegate method if initially successful.

## Discussion

Equivalent to ‘ls’.

