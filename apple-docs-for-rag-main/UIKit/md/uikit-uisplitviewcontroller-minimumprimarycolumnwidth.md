

- UIKit
- UISplitViewController
-  minimumPrimaryColumnWidth 

Instance Property

# minimumPrimaryColumnWidth

The minimum width, in points, for the primary view controller’s content.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var minimumPrimaryColumnWidth: CGFloat { get set }
```

## Discussion

Use this property in conjunction with the maximumPrimaryColumnWidth property to ensure the width of the primary view controller’s content is set to an acceptable value. The preliminary width is specified by the preferredPrimaryColumnWidthFraction property, which is applied to the split view controller’s width and checked against these bounds. If the resulting width is less than the minimum value specified by this property, the width is set to the value in this property.

The default value of this property is automaticDimension, which corresponds to a minimum width of 0 points.

## See Also

### Managing column dimensions

var isCollapsed: Bool

A Boolean value that indicates whether only one of the child view controllers displays.

var preferredPrimaryColumnWidthFraction: CGFloat

The relative width of the primary view controller’s content.

var preferredPrimaryColumnWidth: CGFloat

The preferred width, in points, of the primary view controller’s content.

var primaryColumnWidth: CGFloat

The width, in points, of the primary view controller’s content.

var maximumPrimaryColumnWidth: CGFloat

The maximum width, in points, for the primary view controller’s content.

var preferredSupplementaryColumnWidthFraction: CGFloat

The relative width of the supplementary view controller’s content.

var preferredSupplementaryColumnWidth: CGFloat

The preferred width, in points, of the supplementary view controller’s content.

var supplementaryColumnWidth: CGFloat

The width, in points, of the supplementary view controller’s content.

var minimumSupplementaryColumnWidth: CGFloat

The minimum width, in points, for the supplementary view controller’s content.

var maximumSupplementaryColumnWidth: CGFloat

The maximum width, in points, for the supplementary view controller’s content.

class let automaticDimension: CGFloat

The default value to apply to a dimension.

