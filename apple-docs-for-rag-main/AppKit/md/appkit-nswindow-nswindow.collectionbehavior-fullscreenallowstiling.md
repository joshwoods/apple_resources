

- AppKit
- NSWindow
- NSWindow.CollectionBehavior
-  fullScreenAllowsTiling 

Type Property

# fullScreenAllowsTiling

The window can be a secondary full screen tile even if it can’t be a full screen window itself.

macOS 10.11+

``` source
static var fullScreenAllowsTiling: NSWindow.CollectionBehavior { get }
```

## Discussion

The default behavior is to allow any window to participate in full-screen tiling, as long as it isn’t a panel or sheet and it meets certain requirements, such as being resizable. Windows that aren’t full screen capable can still become a secondary tile in full-screen.

A window can explicitly allow the system to place the window into a full-screen tile by including fullScreenAllowsTiling. Even if a window allows full-screen tiling, the system may not put it in the tile if the window’s minFullScreenContentSize is too large.

A window can explicitly disallow the system from placing the window in a full-screen tile by including fullScreenDisallowsTiling. Windows that don’t support full-screen mode can use fullScreenDisallowsTiling to prevent the system from putting the window into a full-screen tile. Full-screen windows can use fullScreenDisallowsTiling to prevent the system from placing any other windows in its full-screen tile.

Note

The system raises an exception if you set both fullScreenAllowsTiling and fullScreenDisallowsTiling.

## See Also

### Full screen

static var fullScreenPrimary: NSWindow.CollectionBehavior

The window can enter full-screen mode.

static var fullScreenAuxiliary: NSWindow.CollectionBehavior

The window displays on the same space as the full screen window.

static var fullScreenNone: NSWindow.CollectionBehavior

The window doesn’t support full-screen mode.

static var fullScreenDisallowsTiling: NSWindow.CollectionBehavior

The window doesn’t support being a full-screen tile window, but may support being a full-screen window.

