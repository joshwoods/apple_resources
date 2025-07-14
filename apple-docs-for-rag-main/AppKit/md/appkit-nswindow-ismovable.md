

- AppKit
- NSWindow
-  isMovable 

Instance Property

# isMovable

A Boolean value that indicates whether the window can be dragged by clicking in its title bar or background.

macOS 10.6+

``` source
@MainActor
var isMovable: Bool { get set }
```

## Discussion

The value of this property is true if the window can be moved by the user; otherwise, false.

When a window’s isMovable property is false, the value of the isMovableByWindowBackground property is ignored. When the value of isMovable is false, the window can only be dragged between spaces in F8 mode, and its relative screen position is always preserved. Note that a resizable window may still be resized, and the window frame may be changed programmatically. A nonmovable window will not be moved or resized by the system in response to a display reconfiguration. Applications may choose to enable application-controlled window dragging after disabling user-initiating dragging by handling the mouseDown(with:)/mouseDragged(with:)/mouseUp(with:) sequence in sendEvent(_:) in an `NSWindow` subclass.

## See Also

### Moving Windows

var isMovableByWindowBackground: Bool

A Boolean value that indicates whether the window is movable by clicking and dragging anywhere in its background.

func center()

Sets the window’s location to the center of the screen.

