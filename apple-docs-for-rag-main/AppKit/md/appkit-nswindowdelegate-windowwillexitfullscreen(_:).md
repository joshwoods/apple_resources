

- AppKit
- NSWindowDelegate
-  windowWillExitFullScreen(\_:) 

Instance Method

# windowWillExitFullScreen(\_:)

The window is about to exit full-screen mode.

macOS 10.7+

``` source
@MainActor
optional func windowWillExitFullScreen(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named willExitFullScreenNotification.

## See Also

### Managing Full-Screen Presentation

func window(NSWindow, willUseFullScreenContentSize: NSSize) -> NSSize

Called to allow the delegate to modify the full-screen content size.

func window(NSWindow, willUseFullScreenPresentationOptions: NSApplication.PresentationOptions) -> NSApplication.PresentationOptions

Returns the presentation options the window uses when transitioning to full-screen mode.

func windowWillEnterFullScreen(Notification)

The window is about to enter full-screen mode.

func windowDidEnterFullScreen(Notification)

The window has entered full-screen mode.

func windowDidExitFullScreen(Notification)

The window has left full-screen mode.

