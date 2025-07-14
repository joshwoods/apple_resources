

- Core NFC
- NFCISO15693Tag
-  sendCustomCommand(commandConfiguration:completionHandler:) 

Instance Method

# sendCustomCommand(commandConfiguration:completionHandler:)

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
func sendCustomCommand(
    commandConfiguration: NFCISO15693CustomCommandConfiguration,
    completionHandler: @escaping (Data, (any Error)?) -> Void
)
```

**Required**

## Parameters 

`commandConfiguration`  

Configuration for the Manufacturer Custom Command.

`completionHandler`  

Completion handler called when the operation is completed. error is nil if operation succeeds. A @link NFCISO15693TagResponseErrorKey @link/ in NSError userInfo dictionary is returned when the tag responded to the command with an error, and the error code value is defined in ISO15693-3 specification.

## Discussion

Send a manufacturer dependent custom command using command code range from 0xA0 to 0xDF. Refer to ISO15693-3 specification for details.

