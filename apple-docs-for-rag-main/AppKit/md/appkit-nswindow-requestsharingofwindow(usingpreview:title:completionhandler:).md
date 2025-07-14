

- AppKit
- NSWindow
-  requestSharingOfWindow(usingPreview:title:completionHandler:) 

Instance Method

# requestSharingOfWindow(usingPreview:title:completionHandler:)

macOS 15.0+

``` source
@MainActor
func requestSharingOfWindow(
    usingPreview image: NSImage,
    title: String,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
@MainActor
func requestSharingOfWindow(
    usingPreview image: NSImage,
    title: String
) async throws
```

## Parameters 

`title`  

The title to show in a confirmation dialog

`completionHandler`  

A completion block that is called after the request finishes.

## Discussion

An image showing a preview of the window to share

The error will be non-nil if the request does not result in a window being shared. The error will be NSUserCancelledError if there is no ScreenCaptureKit session, or if the user rejects the offer to share. If sharing fails for some other reason, the error will provide the details.

