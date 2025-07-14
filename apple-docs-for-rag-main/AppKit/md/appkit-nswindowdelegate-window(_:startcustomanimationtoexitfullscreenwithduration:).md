

- AppKit
- NSWindowDelegate
-  window(\_:startCustomAnimationToExitFullScreenWithDuration:) 

Instance Method

# window(\_:startCustomAnimationToExitFullScreenWithDuration:)

This method is called to start the window animation out of full-screen mode, including transitioning back to the desktop space.

macOS 10.7+

``` source
@MainActor
optional func window(
    _ window: NSWindow,
    startCustomAnimationToExitFullScreenWithDuration duration: TimeInterval
)
```

## Parameters 

`window`  

The window to exit to full-screen mode.

`duration`  

The duration of the presentation change.

## Discussion

You can implement this method to perform custom animation with the given duration to be in sync with the system animation.

### Special Considerations

This method is called only if customWindowsToExitFullScreen(for:) returns non-`nil`.

## See Also

### Custom Full-Screen Presentation Animations

func customWindowsToEnterFullScreen(for: NSWindow) -> [NSWindow]?

Called when the window is about to enter full-screen mode.

func customWindowsToEnterFullScreen(for: NSWindow, on: NSScreen) -> [NSWindow]?

Called when the window is about to enter full-screen mode.

func window(NSWindow, startCustomAnimationToEnterFullScreenWithDuration: TimeInterval)

This method is called to start the window animation into full-screen mode, including transitioning to a new space.

func window(NSWindow, startCustomAnimationToEnterFullScreenOn: NSScreen, withDuration: TimeInterval)

This method is called to start the window animation into full-screen mode, including transitioning to a new space.

func windowDidFailToEnterFullScreen(NSWindow)

Called if the window failed to enter full-screen mode.

func customWindowsToExitFullScreen(for: NSWindow) -> [NSWindow]?

Called when the window is about to exit full-screen mode.

func windowDidFailToExitFullScreen(NSWindow)

Called if the window failed to exit full-screen mode.

