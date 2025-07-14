

- AppKit
- NSWindow
-  requestSharingOfWindow(\_:completionHandler:) 

Instance Method

# requestSharingOfWindow(\_:completionHandler:)

macOS 15.0+

``` source
@MainActor
func requestSharingOfWindow(
    _ window: NSWindow,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
@MainActor
func requestSharingOfWindow(_ window: NSWindow) async throws
```

## Parameters 

`completionHandler`  

A completion block that is called after the request finishes.

## Discussion

The window to share

The error will be non-nil if the request does not result in a window being shared. The error will be NSUserCancelledError if there is no ScreenCaptureKit session, or if the user rejects the offer to share. If sharing fails for some other reason, the error will provide the details.

