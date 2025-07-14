

- AppKit
- NSWindowDelegate
-  windowDidFailToExitFullScreen(\_:) 

Instance Method

# windowDidFailToExitFullScreen(\_:)

Called if the window failed to exit full-screen mode.

macOS 10.7+

``` source
@MainActor
optional func windowDidFailToExitFullScreen(_ window: NSWindow)
```

## Parameters 

`window`  

The window that failed to exit to full-screen mode.

## Discussion

In some cases, the transition to exit full-screen mode can fail, due to being in the midst of handling some other animation or user gesture. This method indicates that there was an error, and you should clean up any work you may have done to prepare to exit full-screen mode.

This message is sent whether or not the delegate indicated a custom animation by returning non-`nil` from customWindowsToExitFullScreen(for:).

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

func window(NSWindow, startCustomAnimationToExitFullScreenWithDuration: TimeInterval)

This method is called to start the window animation out of full-screen mode, including transitioning back to the desktop space.

