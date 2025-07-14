

- UIKit
- UISplitViewController
-  isCollapsed 

Instance Property

# isCollapsed

A Boolean value that indicates whether only one of the child view controllers displays.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isCollapsed: Bool { get }
```

## Discussion

This property is set to true when the split view controller content is semantically collapsed into a single container. Collapsing happens when the split view controller transitions from a horizontally regular to a horizontally compact environment. After it has been collapsed, the split view controller reports having only one child view controller in its viewControllers property. When collapsed, the displayMode property has no impact on the appearance of the split view interface.

In a column-style split view interface, if this property is true and the split view controller has a view controller set for its UISplitViewController.Column.compact column, the interface displays that view controller.

The value of this property is false when the split view controller is capable of displaying more than one of its child view controllers at the same time, even if it’s not showing more than one at the moment. In this expanded mode, the split view controller’s configuration of its child view controllers is determined by the displayMode property.

During a transition from an expanded to a collapsed interface, the value of this property is false until after the collapse transition finishes and all of the relevant delegate methods have been called. Similarly, when transitioning back to an expanded interface, the value is true until the transition finishes.

## See Also

### Managing column dimensions

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

