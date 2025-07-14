

- AppKit
- NSWindow
- NSWindow.CollectionBehavior
-  fullScreenNone 

Type Property

# fullScreenNone

The window doesn’t support full-screen mode.

macOS 10.7+

``` source
static var fullScreenNone: NSWindow.CollectionBehavior { get }
```

## See Also

### Full screen

static var fullScreenPrimary: NSWindow.CollectionBehavior

The window can enter full-screen mode.

static var fullScreenAuxiliary: NSWindow.CollectionBehavior

The window displays on the same space as the full screen window.

static var fullScreenAllowsTiling: NSWindow.CollectionBehavior

The window can be a secondary full screen tile even if it can’t be a full screen window itself.

static var fullScreenDisallowsTiling: NSWindow.CollectionBehavior

The window doesn’t support being a full-screen tile window, but may support being a full-screen window.

