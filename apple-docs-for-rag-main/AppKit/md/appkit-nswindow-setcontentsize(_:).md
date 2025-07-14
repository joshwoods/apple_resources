

- AppKit
- NSWindow
-  setContentSize(\_:) 

Instance Method

# setContentSize(\_:)

Sets the size of the window’s content view to a given size, which is expressed in the window’s base coordinate system.

macOS

``` source
@MainActor
func setContentSize(_ size: NSSize)
```

## Parameters 

`size`  

The new size of the window’s content view in the window’s base coordinate system.

## Discussion

This size in turn alters the size of the `NSWindow` object itself. Note that the window server limits window sizes to 10,000; if necessary, be sure to limit `aSize` relative to the frame rectangle.

## See Also

### Related Documentation

func setFrame(NSRect, display: Bool)

Sets the origin and size of the window’s frame rectangle according to a given frame rectangle, thereby setting its position and size onscreen.

class func frameRect(forContentRect: NSRect, styleMask: NSWindow.StyleMask) -> NSRect

Returns the frame rectangle used by a window with a given content rectangle and window style.

class func contentRect(forFrameRect: NSRect, styleMask: NSWindow.StyleMask) -> NSRect

Returns the content rectangle used by a window with a given frame rectangle and window style.

### Sizing Content

var contentAspectRatio: NSSize

The window’s content aspect ratio.

var contentMinSize: NSSize

The minimum size of the window’s content view in the window’s base coordinate system.

var contentMaxSize: NSSize

The maximum size of the window’s content view in the window’s base coordinate system.

var contentResizeIncrements: NSSize

The window’s content-view resizing increments.

var contentLayoutGuide: Any?

A value used by Auto Layout constraints to automatically bind to the value of contentLayoutRect.

var contentLayoutRect: NSRect

The area inside the window that is for non-obscured content, in window coordinates.

var maxFullScreenContentSize: NSSize

A maximum size that is used to determine if a window can fit when it is in full screen in a tile.

var minFullScreenContentSize: NSSize

A minimum size that is used to determine if a window can fit when it is in full screen in a tile.

