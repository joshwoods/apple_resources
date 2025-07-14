

- AppKit
- NSView
-  layout() 

Instance Method

# layout()

Perform layout in concert with the constraint-based layout system.

macOS 10.7+

``` source
@MainActor
func layout()
```

## Discussion

Override this method if your custom view needs to perform custom layout not expressible using the constraint-based layout system. In this case you are responsible for setting needsLayout to true when something that impacts your custom layout changes.

You may not invalidate any constraints as part of your layout phase, nor invalidate the layout of your superview or views outside of your view hierarchy. You also may not invoke a drawing pass as part of layout.

You must call `[super layout]` as part of your implementation.

## See Also

### Triggering Auto Layout

var needsLayout: Bool

A Boolean value indicating whether the view needs a layout pass before it can be drawn.

func layoutSubtreeIfNeeded()

Updates the layout of the receiving view and its subviews based on the current views and constraints.

var needsUpdateConstraints: Bool

A Boolean value indicating whether the view’s constraints need to be updated.

func updateConstraints()

Update constraints for the view.

func updateConstraintsForSubtreeIfNeeded()

Updates the constraints for the receiving view and its subviews.

