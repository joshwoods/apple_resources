

- AppKit
- NSSplitViewItem
- NSSplitViewItem.CollapseBehavior
-  NSSplitViewItem.CollapseBehavior.useConstraints 

Case

# NSSplitViewItem.CollapseBehavior.useConstraints

The item collapses and expands using a constraint animation, with a constraint priority of the item’s holding priority.

macOS 10.11+

``` source
case useConstraints
```

## Discussion

This collapse behavior may result in a partial internal content resize and window resize, and doesn’t affect whether the window stays onscreen. You can use external constraints to adjust how the animation affects the item, its sibling items, and the window’s size and position.

## See Also

### Constants

case `default`

The item uses the default collapsing behavior.

case preferResizingSplitViewWithFixedSiblings

The item’s preference is to keep the other panes at their current size and position onscreen, potentially growing or shrinking the window in the direction to best preserve that.

case preferResizingSiblingsWithFixedSplitView

The item’s preference is to resize the other split panes.

