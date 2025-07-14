

- Safari Services
- SFSafariApplication
-  dispatchMessage(withName:toExtensionWithIdentifier:userInfo:completionHandler:) 

Type Method

# dispatchMessage(withName:toExtensionWithIdentifier:userInfo:completionHandler:)

Sends a message to a Safari app extension, launching Safari if necessary.

macOS 10.12.4+

``` source
class func dispatchMessage(
    withName messageName: String,
    toExtensionWithIdentifier identifier: String,
    userInfo: [String : Any]? = nil,
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
class func dispatchMessage(
    withName messageName: String,
    toExtensionWithIdentifier identifier: String,
    userInfo: [String : Any]? = nil
) async throws
```

## Parameters 

`messageName`  

A string that identifies the message.

`identifier`  

The bundle identifier for the app extension.

`userInfo`  

Optional message content.

`completionHandler`  

A completion handler called when the task completes.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
class func dispatchMessage(withName messageName: String, toExtensionWithIdentifier identifier: String, userInfo: [String : Any]? = nil) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

This method may be called only from the app that contains your Safari app extension. If your extension is disabled, nothing happens. If it is enabled, the message is delivered to your app extension. If necessary, this call ensures that Safari is launched and that your extension is running before delivering the message.

Note

The message is sent to the user’s default version of Safari. For example, if a user has selected Safari Technology Preview as the default version on their system, the preview version is launched to receive the message.

