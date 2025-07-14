

- AppKit
- NSWindow
-  isMovableByWindowBackground 

Instance Property

# isMovableByWindowBackground

A Boolean value that indicates whether the window is movable by clicking and dragging anywhere in its background.

macOS

``` source
@MainActor
var isMovableByWindowBackground: Bool { get set }
```

## Discussion

The value of this property is true when the window is movable by clicking and dragging anywhere in its background; otherwise, false.

A window with a style mask of `NSTexturedBackgroundWindowMask` is movable by background by default. Sheets and drawers cannot be movable by window background.

## See Also

### Moving Windows

var isMovable: Bool

A Boolean value that indicates whether the window can be dragged by clicking in its title bar or background.

func center()

Sets the window’s location to the center of the screen.

