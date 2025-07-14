

- Safari Services
- SFSafariApplication
-  openWindow(with:completionHandler:) 

Type Method

# openWindow(with:completionHandler:)

Opens a new window with the desired webpage.

macOS 10.12+

``` source
class func openWindow(
    with url: URL,
    completionHandler: ((SFSafariWindow?) -> Void)? = nil
)
```

``` source
class func openWindow(with url: URL) async -> SFSafariWindow?
```

## Parameters 

`url`  

The URL to navigate to. The URL scheme must be `http` or `https`.

`completionHandler`  

A block to call when the URL is loaded in a new window.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
class func openWindow(with url: URL) async -> SFSafariWindow?
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Working with Windows

class func getActiveWindow(completionHandler: (SFSafariWindow?) -> Void)

Calls the completion handler with the active browser window.

class func showPreferencesForExtension(withIdentifier: String, completionHandler: (((any Error)?) -> Void)?)

Launches Safari and opens the preferences panel for a Safari app extension.

