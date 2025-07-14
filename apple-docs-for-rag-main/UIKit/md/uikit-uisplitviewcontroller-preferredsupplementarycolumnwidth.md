

- UIKit
- UISplitViewController
-  preferredSupplementaryColumnWidth 

Instance Property

# preferredSupplementaryColumnWidth

The preferred width, in points, of the supplementary view controller’s content.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
var preferredSupplementaryColumnWidth: CGFloat { get set }
```

## Discussion

Use this property to specify your preferred width for the supplementary view controller’s view. The default value of this property is automaticDimension. If you set this property to a value different from automaticDimension, that value takes precedence over preferredSupplementaryColumnWidthFraction.

The values in the minimumSupplementaryColumnWidth and maximumSupplementaryColumnWidth properties constrain the actual width of the supplementary view controller. The split view controller attempts to use the width you specify, but may change this value to accommodate the available space. You can get the actual width for the supplementary view controller’s view from the supplementaryColumnWidth property.

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

var minimumPrimaryColumnWidth: CGFloat

The minimum width, in points, for the primary view controller’s content.

var maximumPrimaryColumnWidth: CGFloat

The maximum width, in points, for the primary view controller’s content.

var preferredSupplementaryColumnWidthFraction: CGFloat

The relative width of the supplementary view controller’s content.

var supplementaryColumnWidth: CGFloat

The width, in points, of the supplementary view controller’s content.

var minimumSupplementaryColumnWidth: CGFloat

The minimum width, in points, for the supplementary view controller’s content.

var maximumSupplementaryColumnWidth: CGFloat

The maximum width, in points, for the supplementary view controller’s content.

class let automaticDimension: CGFloat

The default value to apply to a dimension.

