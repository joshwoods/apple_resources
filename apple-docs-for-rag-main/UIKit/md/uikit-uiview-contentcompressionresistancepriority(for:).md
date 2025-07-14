

- UIKit
- UIView
-  contentCompressionResistancePriority(for:) 

Instance Method

# contentCompressionResistancePriority(for:)

Returns the priority with which a view resists being made smaller than its intrinsic size.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func contentCompressionResistancePriority(for axis: NSLayoutConstraint.Axis) -> UILayoutPriority
```

## Parameters 

`axis`  

The axis of the view that might be reduced.

## Return Value

The priority with which the view should resist being compressed from its intrinsic size on the specified axis.

## Discussion

The constraint-based layout system uses these priorities when determining the best layout for views that are encountering constraints that would require them to be smaller than their intrinsic size.

Subclasses should not override this method. Instead, custom views should set default values for their content on creation, typically to `UILayoutPriorityDefaultLow` or `UILayoutPriorityDefaultHigh`.

## See Also

### Measuring in Auto Layout

func systemLayoutSizeFitting(CGSize) -> CGSize

Returns the optimal size of the view based on its current constraints.

func systemLayoutSizeFitting(CGSize, withHorizontalFittingPriority: UILayoutPriority, verticalFittingPriority: UILayoutPriority) -> CGSize

Returns the optimal size of the view based on its constraints and the specified fitting priorities.

var intrinsicContentSize: CGSize

The natural size for the receiving view, considering only properties of the view itself.

func invalidateIntrinsicContentSize()

Invalidates the view’s intrinsic content size.

func setContentCompressionResistancePriority(UILayoutPriority, for: NSLayoutConstraint.Axis)

Sets the priority with which a view resists being made smaller than its intrinsic size.

func contentHuggingPriority(for: NSLayoutConstraint.Axis) -> UILayoutPriority

Returns the priority with which a view resists being made larger than its intrinsic size.

func setContentHuggingPriority(UILayoutPriority, for: NSLayoutConstraint.Axis)

Sets the priority with which a view resists being made larger than its intrinsic size.

