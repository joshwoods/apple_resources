

- UIKit
- UIView
-  systemLayoutSizeFitting(\_:withHorizontalFittingPriority:verticalFittingPriority:) 

Instance Method

# systemLayoutSizeFitting(\_:withHorizontalFittingPriority:verticalFittingPriority:)

Returns the optimal size of the view based on its constraints and the specified fitting priorities.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func systemLayoutSizeFitting(
    _ targetSize: CGSize,
    withHorizontalFittingPriority horizontalFittingPriority: UILayoutPriority,
    verticalFittingPriority: UILayoutPriority
) -> CGSize
```

## Parameters 

`targetSize`  

The size that you prefer for the view. To obtain a view that is as small as possible, specify the constant layoutFittingCompressedSize. To obtain a view that is as large as possible, specify the constant layoutFittingExpandedSize.

`horizontalFittingPriority`  

The priority for horizontal constraints. Specify fittingSizeLevel to get a width that is as close as possible to the width value of `targetSize`.

`verticalFittingPriority`  

The priority for vertical constraints. Specify fittingSizeLevel to get a height that is as close as possible to the height value of `targetSize`.

## Return Value

The optimal size for the view based on the provided constraint priorities.

## Discussion

Use this method when you want to prioritize the view’s constraints when determining the best possible size of the view. This method does not actually change the size of the view.

## See Also

### Measuring in Auto Layout

func systemLayoutSizeFitting(CGSize) -> CGSize

Returns the optimal size of the view based on its current constraints.

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

func setContentHuggingPriority(UILayoutPriority, for: NSLayoutConstraint.Axis)

Sets the priority with which a view resists being made larger than its intrinsic size.

