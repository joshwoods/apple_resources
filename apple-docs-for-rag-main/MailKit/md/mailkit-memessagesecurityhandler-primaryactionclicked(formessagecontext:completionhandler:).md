

- MailKit
- MEMessageSecurityHandler
-  primaryActionClicked(forMessageContext:completionHandler:) 

Instance Method

# primaryActionClicked(forMessageContext:completionHandler:)

macOS 12.0+

``` source
@MainActor
func primaryActionClicked(
    forMessageContext context: Data,
    completionHandler: @escaping (MEExtensionViewController?) -> Void
)
```

``` source
@MainActor
func primaryActionClicked(forMessageContext context: Data) async -> MEExtensionViewController?
```

**Required**

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func primaryActionClicked(forMessageContext context: Data) async -> MEExtensionViewController?
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Instance Methods

func extensionViewController(messageContext: Data) -> MEExtensionViewController?

**Required**

