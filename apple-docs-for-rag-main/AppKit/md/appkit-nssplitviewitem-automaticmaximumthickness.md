

- AppKit
- NSSplitViewItem
-  automaticMaximumThickness 

Instance Property

# automaticMaximumThickness

The maximum thickness of the split view item when it resizes due to automatic sizing.

macOS 10.11+

``` source
var automaticMaximumThickness: CGFloat { get set }
```

## Discussion

Automatic sizing may happen when the split view item has a set preferredThicknessFraction and the app enters full-screen mode, or when other split view items cause the item to change size. The user can still resize the item up to its absolute maximum size in maximumThickness by dragging the divider.

The default value of this property is unspecifiedDimension, which means the split view item doesn’t enforce an automatic maximum size.

## See Also

### Managing the Item Thickness

var preferredThicknessFraction: CGFloat

The preferred thickness of the split view item relative to the split view.

var minimumThickness: CGFloat

The minimum thickness of the split view item.

var maximumThickness: CGFloat

The maximum thickness of the split view item.

class let unspecifiedDimension: CGFloat

A constant that resets a dimension’s value.

