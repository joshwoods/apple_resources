

- AppKit
- NSSplitViewItem
-  holdingPriority 

Instance Property

# holdingPriority

The priority for a split view item to hold its size.

macOS 10.10+

``` source
var holdingPriority: NSLayoutConstraint.Priority { get set }
```

## Discussion

This priority affects the split view item’s width (for a vertical split view) or height (for a horizontal split view).

The view with the lowest priority is the first to gain additional width if the split view grows or shrinks. The default of this property is defaultLow.

