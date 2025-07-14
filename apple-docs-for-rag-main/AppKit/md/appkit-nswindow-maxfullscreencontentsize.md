

- AppKit
- NSWindow
-  maxFullScreenContentSize 

Instance Property

# maxFullScreenContentSize

A maximum size that is used to determine if a window can fit when it is in full screen in a tile.

macOS 10.11+

``` source
@MainActor
var maxFullScreenContentSize: NSSize { get set }
```

## Discussion

By default, the system uses Auto Layout to determine the maximum size, so applications that don’t change window content upon entering full screen should not need to set the value of maxFullScreenContentSize. (If Auto Layout is not used, the system queries contentMinSize and contentMaxSize.) If an application does significant rework of the user interface in full screen, then it may be necessary to set the value of maxFullScreenContentSize. You can use this property even if the window does not support full screen, but can be implicitly opted into supporting a full screen tile based on resizing behavior and window properties (for more information, see the collectionBehavior property).

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

var contentLayoutGuide: Any?

A value used by Auto Layout constraints to automatically bind to the value of contentLayoutRect.

var contentLayoutRect: NSRect

The area inside the window that is for non-obscured content, in window coordinates.

var minFullScreenContentSize: NSSize

A minimum size that is used to determine if a window can fit when it is in full screen in a tile.

