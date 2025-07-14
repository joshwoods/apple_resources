

- MailKit
- MEExtensionManager
-  reloadContentBlocker(withIdentifier:completionHandler:) 

Type Method

# reloadContentBlocker(withIdentifier:completionHandler:)

macOS 12.0+

``` source
class func reloadContentBlocker(
    withIdentifier identifier: String,
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
class func reloadContentBlocker(withIdentifier identifier: String) async throws
```

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
class func reloadContentBlocker(withIdentifier identifier: String) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Type Methods

class func reloadVisibleMessages(completionHandler: (((any Error)?) -> Void)?)

