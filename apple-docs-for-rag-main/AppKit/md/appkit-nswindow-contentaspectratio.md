

- AppKit
- NSWindow
-  contentAspectRatio 

Instance Property

# contentAspectRatio

The window’s content aspect ratio.

macOS

``` source
@MainActor
var contentAspectRatio: NSSize { get set }
```

## Discussion

By default, the content aspect ratio (that is, height in relation to width) is `(0, 0)`. If you set the aspect ratio of a window’s content view, the dimensions of its content rectangle are constrained to integral multiples of that ratio when users resize it. You can set a window’s content view to any size programmatically, regardless of its aspect ratio. The value of this property takes precedence over aspectRatio.

## See Also

### Sizing Content

var contentMinSize: NSSize

The minimum size of the window’s content view in the window’s base coordinate system.

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

