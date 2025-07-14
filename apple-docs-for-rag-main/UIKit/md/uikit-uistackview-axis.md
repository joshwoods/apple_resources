

- UIKit
- UIStackView
-  axis 

Instance Property

# axis

The axis along which the arranged views lay out.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var axis: NSLayoutConstraint.Axis { get set }
```

## Discussion

This property determines the orientation of the arranged views. Assigning the NSLayoutConstraint.Axis.vertical value creates a column of views. Assigning the NSLayoutConstraint.Axis.horizontal value creates a row. The default value is NSLayoutConstraint.Axis.horizontal.

## See Also

### Configuring the layout

var alignment: UIStackView.Alignment

The alignment of the arranged subviews perpendicular to the stack view’s axis.

var distribution: UIStackView.Distribution

The distribution of the arranged views along the stack view’s axis.

var spacing: CGFloat

The distance in points between the adjacent edges of the stack view’s arranged views.

var isBaselineRelativeArrangement: Bool

A Boolean value that determines whether the vertical spacing between views is measured from their baselines.

var isLayoutMarginsRelativeArrangement: Bool

A Boolean value that determines whether the stack view lays out its arranged views relative to its layout margins.

