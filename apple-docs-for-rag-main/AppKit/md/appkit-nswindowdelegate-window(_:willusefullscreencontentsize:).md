

- AppKit
- NSWindowDelegate
-  window(\_:willUseFullScreenContentSize:) 

Instance Method

# window(\_:willUseFullScreenContentSize:)

Called to allow the delegate to modify the full-screen content size.

macOS 10.7+

``` source
@MainActor
optional func window(
    _ window: NSWindow,
    willUseFullScreenContentSize proposedSize: NSSize
) -> NSSize
```

## Parameters 

`window`  

The window to enter to full-screen mode.

`proposedSize`  

The proposed window size.

## Return Value

The window size to use when displaying content size.

## See Also

### Managing Full-Screen Presentation

func window(NSWindow, willUseFullScreenPresentationOptions: NSApplication.PresentationOptions) -> NSApplication.PresentationOptions

Returns the presentation options the window uses when transitioning to full-screen mode.

func windowWillEnterFullScreen(Notification)

The window is about to enter full-screen mode.

func windowDidEnterFullScreen(Notification)

The window has entered full-screen mode.

func windowWillExitFullScreen(Notification)

The window is about to exit full-screen mode.

func windowDidExitFullScreen(Notification)

The window has left full-screen mode.

