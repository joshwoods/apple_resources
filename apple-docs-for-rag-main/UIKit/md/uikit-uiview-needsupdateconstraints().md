

- UIKit
- UIView
-  needsUpdateConstraints() 

Instance Method

# needsUpdateConstraints()

A Boolean value that determines whether the view’s constraints need updating.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func needsUpdateConstraints() -> Bool
```

## Return Value

true if the view’s constraints need updating, false otherwise.

## Discussion

The constraint-based layout system uses the return value of this method to determine whether it needs to call updateConstraints() on your view as part of its normal layout pass.

## See Also

### Triggering Auto Layout

func setNeedsUpdateConstraints()

Controls whether the view’s constraints need updating.

func updateConstraints()

Updates constraints for the view.

func updateConstraintsIfNeeded()

Updates the constraints for the receiving view and its subviews.

