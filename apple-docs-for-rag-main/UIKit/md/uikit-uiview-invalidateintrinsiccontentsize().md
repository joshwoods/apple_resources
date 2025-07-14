

- UIKit
- UIView
-  invalidateIntrinsicContentSize() 

Instance Method

# invalidateIntrinsicContentSize()

Invalidates the view’s intrinsic content size.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func invalidateIntrinsicContentSize()
```

## Discussion

Call this when something changes in your custom view that invalidates its intrinsic content size. This allows the constraint-based layout system to take the new intrinsic content size into account in its next layout pass.

## See Also

### Measuring in Auto Layout

func systemLayoutSizeFitting(CGSize) -> CGSize

Returns the optimal size of the view based on its current constraints.

func systemLayoutSizeFitting(CGSize, withHorizontalFittingPriority: UILayoutPriority, verticalFittingPriority: UILayoutPriority) -> CGSize

Returns the optimal size of the view based on its constraints and the specified fitting priorities.

var intrinsicContentSize: CGSize

The natural size for the receiving view, considering only properties of the view itself.

func contentCompressionResistancePriority(for: NSLayoutConstraint.Axis) -> UILayoutPriority

Returns the priority with which a view resists being made smaller than its intrinsic size.

func setContentCompressionResistancePriority(UILayoutPriority, for: NSLayoutConstraint.Axis)

Sets the priority with which a view resists being made smaller than its intrinsic size.

func contentHuggingPriority(for: NSLayoutConstraint.Axis) -> UILayoutPriority

Returns the priority with which a view resists being made larger than its intrinsic size.

func setContentHuggingPriority(UILayoutPriority, for: NSLayoutConstraint.Axis)

Sets the priority with which a view resists being made larger than its intrinsic size.

