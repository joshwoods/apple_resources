

- AppKit
- NSStackView
- NSStackView.VisibilityPriority
-  detachOnlyIfNecessary 

Type Property

# detachOnlyIfNecessary

The Auto Layout priority that results in detachment of a view when there is insufficient space in the stack view to display it fully.

macOS 10.9+

``` source
static let detachOnlyIfNecessary: NSStackView.VisibilityPriority
```

## See Also

### Type Properties

static let mustHold: NSStackView.VisibilityPriority

The default value, and maximum Auto Layout priority, that results in a view never detaching from the stack view.

static let notVisible: NSStackView.VisibilityPriority

The minimum Auto Layout priority that forces a view to detach from the stack view.

