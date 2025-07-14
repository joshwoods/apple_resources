

- AppKit
- NSSplitViewItem
-  minimumThickness 

Instance Property

# minimumThickness

The minimum thickness of the split view item.

macOS 10.11+

``` source
var minimumThickness: CGFloat { get set }
```

## Discussion

This value affects the split view item’s width (for a vertical split view) or height (for a horizontal split view).

The default value of this property is unspecifiedDimension, which means the split view item doesn’t enforce a minimum size. However, layout constraints in the contained view hierarchy might specify a minimum size regardless.

## See Also

### Managing the Item Thickness

var automaticMaximumThickness: CGFloat

The maximum thickness of the split view item when it resizes due to automatic sizing.

var preferredThicknessFraction: CGFloat

The preferred thickness of the split view item relative to the split view.

var maximumThickness: CGFloat

The maximum thickness of the split view item.

class let unspecifiedDimension: CGFloat

A constant that resets a dimension’s value.

