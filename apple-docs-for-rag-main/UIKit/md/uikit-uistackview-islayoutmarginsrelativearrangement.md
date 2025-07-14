

- UIKit
- UIStackView
-  isLayoutMarginsRelativeArrangement 

Instance Property

# isLayoutMarginsRelativeArrangement

A Boolean value that determines whether the stack view lays out its arranged views relative to its layout margins.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var isLayoutMarginsRelativeArrangement: Bool { get set }
```

## Discussion

If true, the stack view will layout its arranged views relative to its layout margins. If false, it lays out the arranged views relative to its bounds. The default is false.

## See Also

### Configuring the layout

var axis: NSLayoutConstraint.Axis

The axis along which the arranged views lay out.

var alignment: UIStackView.Alignment

The alignment of the arranged subviews perpendicular to the stack view’s axis.

var distribution: UIStackView.Distribution

The distribution of the arranged views along the stack view’s axis.

var spacing: CGFloat

The distance in points between the adjacent edges of the stack view’s arranged views.

var isBaselineRelativeArrangement: Bool

A Boolean value that determines whether the vertical spacing between views is measured from their baselines.

