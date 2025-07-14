

- ReplayKit
- RPBroadcastActivityController
-  showBroadcastPicker(at:from:preferredExtensionIdentifier:completionHandler:) 

Type Method

# showBroadcastPicker(at:from:preferredExtensionIdentifier:completionHandler:)

Presents a list of available broadcast services for the user to select.

macOS 11.0+

``` source
class func showBroadcastPicker(
    at point: CGPoint,
    from window: NSWindow?,
    preferredExtensionIdentifier preferredExtension: String?,
    completionHandler handler: @escaping (RPBroadcastActivityController?, (any Error)?) -> Void
)
```

``` source
class func showBroadcastPicker(
    at point: CGPoint,
    from window: NSWindow?,
    preferredExtensionIdentifier preferredExtension: String?
) async throws -> RPBroadcastActivityController
```

## Parameters 

`point`  

The origin point within the specified window.

`window`  

The window presenting the picker. Specify nil to present the picker from the main app window.

`preferredExtension`  

The extension bundle identifier for the preferred broadcast extension service. Specify nil to show all extensions.

`handler`  

The system calls this closure after the user selects a broadcast extension. The system passes the closure the selected broadcast activity controller, or an error if a failure occurred.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

