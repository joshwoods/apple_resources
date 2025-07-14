

- UIKit
- UIView
-  updateConstraintsIfNeeded() 

Instance Method

# updateConstraintsIfNeeded()

Updates the constraints for the receiving view and its subviews.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func updateConstraintsIfNeeded()
```

## Discussion

Whenever a new layout pass is triggered for a view, the system invokes this method to ensure that any constraints for the view and its subviews are updated with information from the current view hierarchy and its constraints. This method is called automatically by the system, but may be invoked manually if you need to examine the most up to date constraints.

Subclasses should not override this method.

## See Also

### Triggering Auto Layout

func needsUpdateConstraints() -> Bool

A Boolean value that determines whether the view’s constraints need updating.

func setNeedsUpdateConstraints()

Controls whether the view’s constraints need updating.

func updateConstraints()

Updates constraints for the view.

