

- AppKit
- NSWindow
-  contentMinSize 

Instance Property

# contentMinSize

The minimum size of the window’s content view in the window’s base coordinate system.

macOS

``` source
@MainActor
var contentMinSize: NSSize { get set }
```

## Discussion

The minimum size constraint is enforced for resizing by the user as well as for the setContentSize(_:) method and the `setFrame...` methods other than setFrame(_:display:) and setFrame(_:display:animate:). This method takes precedence over the minSize property.

## See Also

### Sizing Content

var contentAspectRatio: NSSize

The window’s content aspect ratio.

func setContentSize(NSSize)

Sets the size of the window’s content view to a given size, which is expressed in the window’s base coordinate system.

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

