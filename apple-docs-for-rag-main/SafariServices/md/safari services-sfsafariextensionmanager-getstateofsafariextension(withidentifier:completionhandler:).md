

- Safari Services
- SFSafariExtensionManager
-  getStateOfSafariExtension(withIdentifier:completionHandler:) 

Type Method

# getStateOfSafariExtension(withIdentifier:completionHandler:)

Gets the current state of the Safari app extension.

macOS 10.12+

``` source
class func getStateOfSafariExtension(
    withIdentifier identifier: String,
    completionHandler: @escaping @MainActor (SFSafariExtensionState?, (any Error)?) -> Void
)
```

``` source
class func stateOfSafariExtension(withIdentifier identifier: String) async throws -> SFSafariExtensionState
```

## Parameters 

`identifier`  

The bundle identifier for the Safari extension to check.

`completionHandler`  

The completion handler the system calls with the Safari extension’s state.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
class func stateOfSafariExtension(withIdentifier identifier: String) async throws -> SFSafariExtensionState
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

This method is used by your app to check on the state of one of the Safari app extensions embedded inside it.

