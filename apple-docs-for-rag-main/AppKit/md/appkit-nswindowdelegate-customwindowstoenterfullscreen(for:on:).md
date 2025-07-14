

- AppKit
- NSWindowDelegate
-  customWindowsToEnterFullScreen(for:on:) 

Instance Method

# customWindowsToEnterFullScreen(for:on:)

Called when the window is about to enter full-screen mode.

macOS 10.9+

``` source
@MainActor
optional func customWindowsToEnterFullScreen(
    for window: NSWindow,
    on screen: NSScreen
) -> [NSWindow]?
```

## Parameters 

`window`  

The window to enter full-screen mode.

`screen`  

The display screen on which the window will enter full-screen mode.

## Return Value

An array of windows to use for the animation to full-screen mode for `window`; otherwise `nil`.

## Discussion

This method lets a window delegate customize the animation when the window is about to enter full-screen mode by providing a custom window or windows containing layers or other effects. If you don’t want to perform custom animation, you can omit the implementation of this method, or it can return `nil`.

### Special Considerations

If this method and customWindowsToEnterFullScreen(for:) are both implemented, this method is called.

## See Also

### Custom Full-Screen Presentation Animations

func customWindowsToEnterFullScreen(for: NSWindow) -> [NSWindow]?

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

func windowDidFailToExitFullScreen(NSWindow)

Called if the window failed to exit full-screen mode.

