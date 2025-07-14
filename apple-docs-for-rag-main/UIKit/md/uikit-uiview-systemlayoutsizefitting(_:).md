

- UIKit
- UIView
-  systemLayoutSizeFitting(\_:) 

Instance Method

# systemLayoutSizeFitting(\_:)

Returns the optimal size of the view based on its current constraints.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func systemLayoutSizeFitting(_ targetSize: CGSize) -> CGSize
```

## Parameters 

`targetSize`  

The size that you prefer for the view. To obtain a view that is as small as possible, specify the constant layoutFittingCompressedSize. To obtain a view that is as large as possible, specify the constant layoutFittingExpandedSize.

## Return Value

The optimal size for the view.

## Discussion

This method returns a size value for the view that optimally satisfies the view’s current constraints and is as close to the value in the `targetSize` parameter as possible. This method does not actually change the size of the view.

## See Also

### Measuring in Auto Layout

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

func setContentHuggingPriority(UILayoutPriority, for: NSLayoutConstraint.Axis)

Sets the priority with which a view resists being made larger than its intrinsic size.

