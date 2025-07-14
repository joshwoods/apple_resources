

- UIKit
- UIView
-  setContentHuggingPriority(\_:for:) 

Instance Method

# setContentHuggingPriority(\_:for:)

Sets the priority with which a view resists being made larger than its intrinsic size.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setContentHuggingPriority(
    _ priority: UILayoutPriority,
    for axis: NSLayoutConstraint.Axis
)
```

## Parameters 

`priority`  

The new priority.

`axis`  

The axis for which the content hugging priority should be set.

## Discussion

Custom views should set default values for both orientations on creation, based on their content, typically to `UILayoutPriorityDefaultLow` or `UILayoutPriorityDefaultHigh`. When creating user interfaces, the layout designer can modify these priorities for specific views when the overall layout design requires different tradeoffs than the natural priorities of the views being used in the interface.

Subclasses should not override this method.

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

func contentCompressionResistancePriority(for: NSLayoutConstraint.Axis) -> UILayoutPriority

Returns the priority with which a view resists being made smaller than its intrinsic size.

func setContentCompressionResistancePriority(UILayoutPriority, for: NSLayoutConstraint.Axis)

Sets the priority with which a view resists being made smaller than its intrinsic size.

func contentHuggingPriority(for: NSLayoutConstraint.Axis) -> UILayoutPriority

Returns the priority with which a view resists being made larger than its intrinsic size.

