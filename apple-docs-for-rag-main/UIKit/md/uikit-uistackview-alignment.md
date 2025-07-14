

- UIKit
- UIStackView
-  alignment 

Instance Property

# alignment

The alignment of the arranged subviews perpendicular to the stack view’s axis.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var alignment: UIStackView.Alignment { get set }
```

## Discussion

This property determines how the stack view lays out its arranged views perpendicularly to its axis. The default value is UIStackView.Alignment.fill. For a list of possible values, see UIStackView.Alignment.

## See Also

### Configuring the layout

var axis: NSLayoutConstraint.Axis

The axis along which the arranged views lay out.

var distribution: UIStackView.Distribution

The distribution of the arranged views along the stack view’s axis.

var spacing: CGFloat

The distance in points between the adjacent edges of the stack view’s arranged views.

var isBaselineRelativeArrangement: Bool

A Boolean value that determines whether the vertical spacing between views is measured from their baselines.

var isLayoutMarginsRelativeArrangement: Bool

A Boolean value that determines whether the stack view lays out its arranged views relative to its layout margins.

