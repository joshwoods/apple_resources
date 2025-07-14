

- AppKit
- NSWindowDelegate
-  window(\_:startCustomAnimationToEnterFullScreenOn:withDuration:) 

Instance Method

# window(\_:startCustomAnimationToEnterFullScreenOn:withDuration:)

This method is called to start the window animation into full-screen mode, including transitioning to a new space.

macOS 10.9+

``` source
@MainActor
optional func window(
    _ window: NSWindow,
    startCustomAnimationToEnterFullScreenOn screen: NSScreen,
    withDuration duration: TimeInterval
)
```

## Parameters 

`window`  

The window to enter full-screen mode.

`screen`  

The display screen on which the window will enter full-screen mode.

`duration`  

The duration of the presentation change.

## Discussion

You can implement this method to perform custom animation with the given duration to be in sync with the system animation.

### Special Considerations

This method is called only if customWindowsToEnterFullScreen(for:) returns non-`nil`. If window(_:startCustomAnimationToEnterFullScreenWithDuration:) and this method are both implemented, this method is called.

## See Also

### Custom Full-Screen Presentation Animations

func customWindowsToEnterFullScreen(for: NSWindow) -> [NSWindow]?

Called when the window is about to enter full-screen mode.

func customWindowsToEnterFullScreen(for: NSWindow, on: NSScreen) -> [NSWindow]?

Called when the window is about to enter full-screen mode.

func window(NSWindow, startCustomAnimationToEnterFullScreenWithDuration: TimeInterval)

This method is called to start the window animation into full-screen mode, including transitioning to a new space.

func windowDidFailToEnterFullScreen(NSWindow)

Called if the window failed to enter full-screen mode.

func customWindowsToExitFullScreen(for: NSWindow) -> [NSWindow]?

Called when the window is about to exit full-screen mode.

func window(NSWindow, startCustomAnimationToExitFullScreenWithDuration: TimeInterval)

This method is called to start the window animation out of full-screen mode, including transitioning back to the desktop space.

func windowDidFailToExitFullScreen(NSWindow)

Called if the window failed to exit full-screen mode.

