

- AppKit
- NSWindow
- NSWindow.CollectionBehavior
-  fullScreenAuxiliary 

Type Property

# fullScreenAuxiliary

The window displays on the same space as the full screen window.

macOS 10.7+

``` source
static var fullScreenAuxiliary: NSWindow.CollectionBehavior { get }
```

## See Also

### Full screen

static var fullScreenPrimary: NSWindow.CollectionBehavior

The window can enter full-screen mode.

static var fullScreenNone: NSWindow.CollectionBehavior

The window doesn’t support full-screen mode.

static var fullScreenAllowsTiling: NSWindow.CollectionBehavior

The window can be a secondary full screen tile even if it can’t be a full screen window itself.

static var fullScreenDisallowsTiling: NSWindow.CollectionBehavior

The window doesn’t support being a full-screen tile window, but may support being a full-screen window.

