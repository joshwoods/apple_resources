

- AppKit
- NSWindow
-  contentLayoutGuide 

Instance Property

# contentLayoutGuide

A value used by Auto Layout constraints to automatically bind to the value of contentLayoutRect.

macOS 10.10+

``` source
@MainActor
var contentLayoutGuide: Any? { get }
```

## See Also

### Sizing Content

var contentAspectRatio: NSSize

The window’s content aspect ratio.

var contentMinSize: NSSize

The minimum size of the window’s content view in the window’s base coordinate system.

func setContentSize(NSSize)

Sets the size of the window’s content view to a given size, which is expressed in the window’s base coordinate system.

var contentMaxSize: NSSize

The maximum size of the window’s content view in the window’s base coordinate system.

var contentResizeIncrements: NSSize

The window’s content-view resizing increments.

var contentLayoutRect: NSRect

The area inside the window that is for non-obscured content, in window coordinates.

var maxFullScreenContentSize: NSSize

A maximum size that is used to determine if a window can fit when it is in full screen in a tile.

var minFullScreenContentSize: NSSize

A minimum size that is used to determine if a window can fit when it is in full screen in a tile.

