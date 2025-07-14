

- AppKit
- NSWindow
-  center() 

Instance Method

# center()

Sets the window’s location to the center of the screen.

macOS

``` source
@MainActor
func center()
```

## Discussion

The window is placed exactly in the center horizontally and somewhat above center vertically. Such a placement carries a certain visual immediacy and importance. This method doesn’t put the window onscreen, however; use makeKeyAndOrderFront(_:) to do that.

You typically use this method to place a window—most likely an alert dialog—where the user can’t miss it. This method is invoked automatically when a panel is placed on the screen by the runModal(for:) method of the `NSApplication` class.

## See Also

### Moving Windows

var isMovableByWindowBackground: Bool

A Boolean value that indicates whether the window is movable by clicking and dragging anywhere in its background.

var isMovable: Bool

A Boolean value that indicates whether the window can be dragged by clicking in its title bar or background.

