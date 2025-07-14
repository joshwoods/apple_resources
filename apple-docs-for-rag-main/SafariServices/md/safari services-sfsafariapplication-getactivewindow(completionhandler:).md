

- Safari Services
- SFSafariApplication
-  getActiveWindow(completionHandler:) 

Type Method

# getActiveWindow(completionHandler:)

Calls the completion handler with the active browser window.

macOS 10.12+

``` source
class func getActiveWindow(completionHandler: @escaping (SFSafariWindow?) -> Void)
```

``` source
class func activeWindow() async -> SFSafariWindow?
```

## Parameters 

`completionHandler`  

A block to call when the active browser window is returned.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
class func activeWindow() async -> SFSafariWindow?
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

If there is no active Safari window, the value of `activeWindow` is `nil`, and the completion handler is not called.

## See Also

### Working with Windows

class func openWindow(with: URL, completionHandler: ((SFSafariWindow?) -> Void)?)

Opens a new window with the desired webpage.

class func showPreferencesForExtension(withIdentifier: String, completionHandler: (((any Error)?) -> Void)?)

Launches Safari and opens the preferences panel for a Safari app extension.

