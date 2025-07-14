

- Safari Services
- SFSafariApplication
-  showPreferencesForExtension(withIdentifier:completionHandler:) 

Type Method

# showPreferencesForExtension(withIdentifier:completionHandler:)

Launches Safari and opens the preferences panel for a Safari app extension.

macOS 10.12+

``` source
class func showPreferencesForExtension(
    withIdentifier identifier: String,
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
class func showPreferencesForExtension(withIdentifier identifier: String) async throws
```

## Parameters 

`identifier`  

The identifier for a Safari app extension in your app bundle.

`completionHandler`  

A completion handler called after the operation completes. The completion handler takes the following parameter:

error  
If an error occurred, this parameter describes the error. If the operation succeeded, this parameter holds `nil`.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
class func showPreferencesForExtension(withIdentifier identifier: String) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Working with Windows

class func getActiveWindow(completionHandler: (SFSafariWindow?) -> Void)

Calls the completion handler with the active browser window.

class func openWindow(with: URL, completionHandler: ((SFSafariWindow?) -> Void)?)

Opens a new window with the desired webpage.

