

- AppKit
- NSWindowDelegate
-  customWindowsToExitFullScreen(for:) 

Instance Method

# customWindowsToExitFullScreen(for:)

Called when the window is about to exit full-screen mode.

macOS 10.7+

``` source
@MainActor
optional func customWindowsToExitFullScreen(for window: NSWindow) -> [NSWindow]?
```

## Parameters 

`window`  

The window to exit full-screen mode.

## Return Value

An array of windows involved in the animation out of full-screen mode for `window`; otherwise `nil`.

## Discussion

This method lets the window delegate customize the animation when the window is about to exit full-screen mode by providing a custom window or windows containing layers or other effects. If an you do not want to perform custom animation, you can omit the implementation of this method, or it can return `nil`.

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

func window(NSWindow, startCustomAnimationToExitFullScreenWithDuration: TimeInterval)

This method is called to start the window animation out of full-screen mode, including transitioning back to the desktop space.

func windowDidFailToExitFullScreen(NSWindow)

Called if the window failed to exit full-screen mode.

