

- CallKit
- CXCallDirectoryManager
-  openSettings(completionHandler:) 

Instance Method

# openSettings(completionHandler:)

Opens the iOS Settings app and shows the Call Blocking & Identification settings.

iOS 13.4+iPadOS 13.4+Mac Catalyst 14.0+visionOS 1.0+

``` source
func openSettings(completionHandler completion: (((any Error)?) -> Void)? = nil)
```

``` source
func openSettings() async throws
```

## Parameters 

`completion`  

A block executed when the manager finishes opening the Call Directory panel.

error  
If an error occurred, an error object indicating how the operation failed; otherwise, `nil`.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func openSettings() async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Before a Call Directory extension can operate on incoming calls, the user must explicitly enable the extension in the iOS Settings app.

Use this method to open the Settings app and show the Call Blocking & Identification settings directly.

