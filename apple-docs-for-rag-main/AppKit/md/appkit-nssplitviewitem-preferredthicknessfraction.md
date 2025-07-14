

- AppKit
- NSSplitViewItem
-  preferredThicknessFraction 

Instance Property

# preferredThicknessFraction

The preferred thickness of the split view item relative to the split view.

macOS 10.11+

``` source
var preferredThicknessFraction: CGFloat { get set }
```

## Discussion

This value represents the proportion of the split view that you want the split view item to occupy on a scale of `0.0` to `1.0`. The system uses this value to adjust the thickness of the item in relation to other items when a user double-clicks a neighboring divider, and when the app enters full-screen mode.

The default value of this property is unspecifiedDimension, which means the item doesn’t resize when a user double-clicks the divider, and the system preserves the absolute size when the app enters full-screen mode.

## See Also

### Managing the Item Thickness

var automaticMaximumThickness: CGFloat

The maximum thickness of the split view item when it resizes due to automatic sizing.

var minimumThickness: CGFloat

The minimum thickness of the split view item.

var maximumThickness: CGFloat

The maximum thickness of the split view item.

class let unspecifiedDimension: CGFloat

A constant that resets a dimension’s value.

