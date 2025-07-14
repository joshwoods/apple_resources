

- AppKit
- NSWindowDelegate
-  windowShouldZoom(\_:toFrame:) 

Instance Method

# windowShouldZoom(\_:toFrame:)

Asks the delegate whether the specified window should zoom to the specified frame.

macOS

``` source
@MainActor
optional func windowShouldZoom(
    _ window: NSWindow,
    toFrame newFrame: NSRect
) -> Bool
```

## Parameters 

`window`  

The window being zoomed.

`newFrame`  

The rectangle to which the specified window is being zoomed.

## Return Value

true to allow `window`’s frame to become `newFrame`; otherwise, false.

## See Also

### Zooming Window

func windowWillUseStandardFrame(NSWindow, defaultFrame: NSRect) -> NSRect

Called by `NSWindow`’s zoom(_:) method while determining the frame a window may be zoomed to.

