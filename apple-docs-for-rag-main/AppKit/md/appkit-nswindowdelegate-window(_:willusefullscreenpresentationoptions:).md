

- AppKit
- NSWindowDelegate
-  window(\_:willUseFullScreenPresentationOptions:) 

Instance Method

# window(\_:willUseFullScreenPresentationOptions:)

Returns the presentation options the window uses when transitioning to full-screen mode.

macOS 10.7+

``` source
@MainActor
optional func window(
    _ window: NSWindow,
    willUseFullScreenPresentationOptions proposedOptions: NSApplication.PresentationOptions = []
) -> NSApplication.PresentationOptions
```

## Parameters 

`window`  

The window to enter to full-screen mode.

`proposedOptions`  

The proposed options. See NSApplication.PresentationOptions for the possible values.

## Return Value

The options the window should use when transitioning to full-screen mode. These may be the same as the `proposedOptions` or may be modified.

## See Also

### Managing Full-Screen Presentation

func window(NSWindow, willUseFullScreenContentSize: NSSize) -> NSSize

Called to allow the delegate to modify the full-screen content size.

func windowWillEnterFullScreen(Notification)

The window is about to enter full-screen mode.

func windowDidEnterFullScreen(Notification)

The window has entered full-screen mode.

func windowWillExitFullScreen(Notification)

The window is about to exit full-screen mode.

func windowDidExitFullScreen(Notification)

The window has left full-screen mode.

