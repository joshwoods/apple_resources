

- MailKit
- MEMessageEncoder
-  getEncodingStatus(for:composeContext:completionHandler:) 

Instance Method

# getEncodingStatus(for:composeContext:completionHandler:)

macOS 12.0+

``` source
func getEncodingStatus(
    for message: MEMessage,
    composeContext: MEComposeContext,
    completionHandler: @escaping (MEOutgoingMessageEncodingStatus) -> Void
)
```

``` source
func encodingStatus(
    for message: MEMessage,
    composeContext: MEComposeContext
) async -> MEOutgoingMessageEncodingStatus
```

**Required**

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func encodingStatus(for message: MEMessage, composeContext: MEComposeContext) async -> MEOutgoingMessageEncodingStatus
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Instance Methods

func encode(MEMessage, composeContext: MEComposeContext, completionHandler: (MEMessageEncodingResult) -> Void)

**Required**

