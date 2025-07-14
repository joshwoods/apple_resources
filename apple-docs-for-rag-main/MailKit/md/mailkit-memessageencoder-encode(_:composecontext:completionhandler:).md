

- MailKit
- MEMessageEncoder
-  encode(\_:composeContext:completionHandler:) 

Instance Method

# encode(\_:composeContext:completionHandler:)

macOS 12.0+

``` source
func encode(
    _ message: MEMessage,
    composeContext: MEComposeContext,
    completionHandler: @escaping (MEMessageEncodingResult) -> Void
)
```

``` source
func encode(
    _ message: MEMessage,
    composeContext: MEComposeContext
) async -> MEMessageEncodingResult
```

**Required**

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func encode(_ message: MEMessage, composeContext: MEComposeContext) async -> MEMessageEncodingResult
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Instance Methods

func getEncodingStatus(for: MEMessage, composeContext: MEComposeContext, completionHandler: (MEOutgoingMessageEncodingStatus) -> Void)

**Required**

