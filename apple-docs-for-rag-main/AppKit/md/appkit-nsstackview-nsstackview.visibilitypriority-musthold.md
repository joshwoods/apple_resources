

- AppKit
- NSStackView
- NSStackView.VisibilityPriority
-  mustHold 

Type Property

# mustHold

The default value, and maximum Auto Layout priority, that results in a view never detaching from the stack view.

macOS 10.9+

``` source
static let mustHold: NSStackView.VisibilityPriority
```

## See Also

### Type Properties

static let detachOnlyIfNecessary: NSStackView.VisibilityPriority

The Auto Layout priority that results in detachment of a view when there is insufficient space in the stack view to display it fully.

static let notVisible: NSStackView.VisibilityPriority

The minimum Auto Layout priority that forces a view to detach from the stack view.

