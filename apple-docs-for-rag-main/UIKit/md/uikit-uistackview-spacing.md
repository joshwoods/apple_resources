

- UIKit
- UIStackView
-  spacing 

Instance Property

# spacing

The distance in points between the adjacent edges of the stack view’s arranged views.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var spacing: CGFloat { get set }
```

## Discussion

This property defines a strict spacing between arranged views for the UIStackView.Distribution.fillProportionally distributions. It represents the minimum spacing for the UIStackView.Distribution.equalSpacing and UIStackView.Distribution.equalCentering distributions. Use negative values to allow overlap. The default value is `0.0`.

## See Also

### Configuring the layout

var axis: NSLayoutConstraint.Axis

The axis along which the arranged views lay out.

var alignment: UIStackView.Alignment

The alignment of the arranged subviews perpendicular to the stack view’s axis.

var distribution: UIStackView.Distribution

The distribution of the arranged views along the stack view’s axis.

var isBaselineRelativeArrangement: Bool

A Boolean value that determines whether the vertical spacing between views is measured from their baselines.

var isLayoutMarginsRelativeArrangement: Bool

A Boolean value that determines whether the stack view lays out its arranged views relative to its layout margins.

