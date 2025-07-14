

- Core NFC
- NFCISO15693Tag
-  readMultipleBlock(readConfiguration:completionHandler:) 

Instance Method

# readMultipleBlock(readConfiguration:completionHandler:)

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
func readMultipleBlock(
    readConfiguration: NFCISO15693ReadMultipleBlocksConfiguration,
    completionHandler: @escaping (Data, (any Error)?) -> Void
)
```

**Required**

## Parameters 

`readConfiguration`  

Configuration For the Read Multiple Blocks command.

`completionHandler`  

Completion handler called when the operation is completed. error is nil if operation succeeds. A @link NFCISO15693TagResponseErrorKey @link/ in NSError userInfo dictionary is returned when the tag responded to the command with an error, and the error code value is defined in ISO15693-3 specification. Successfully read data blocks will be returned from NSData object. All blocks are concatenated into the NSData object.

## Discussion

Performs read operation using Read Multiple Blocks command (0x23 command code) as defined in ISO15693-3 specification. Multiple Read Multiple Blocks commands will be sent if necessary to complete the operation.

