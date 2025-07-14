

- AppKit
- NSWindowDelegate
-  windowForSharingRequest(from:) 

Instance Method

# windowForSharingRequest(from:)

Method called to get the window to share once sharing is confirmed, after a request is initiated by requestSharingOfWindowUsingPreview:title:completionHandler:. Implement this on the delegate of the requesting window

macOS 15.0+

``` source
@MainActor
optional func windowForSharingRequest(from window: NSWindow) -> NSWindow?
```

