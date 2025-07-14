

- AppKit
- NSWindow
- NSWindow.CollectionBehavior
-  fullScreenDisallowsTiling 

Type Property

# fullScreenDisallowsTiling

The window doesn’t support being a full-screen tile window, but may support being a full-screen window.

macOS 10.11+

``` source
static var fullScreenDisallowsTiling: NSWindow.CollectionBehavior { get }
```

## Discussion

For more information about full-screen tile window support, see fullScreenAllowsTiling.

## See Also

### Full screen

static var fullScreenPrimary: NSWindow.CollectionBehavior

The window can enter full-screen mode.

static var fullScreenAuxiliary: NSWindow.CollectionBehavior

The window displays on the same space as the full screen window.

static var fullScreenNone: NSWindow.CollectionBehavior

The window doesn’t support full-screen mode.

static var fullScreenAllowsTiling: NSWindow.CollectionBehavior

The window can be a secondary full screen tile even if it can’t be a full screen window itself.

