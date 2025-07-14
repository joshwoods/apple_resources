

- AppKit
- NSSplitViewItem
- NSSplitViewItem.CollapseBehavior
-  NSSplitViewItem.CollapseBehavior.default 

Case

# NSSplitViewItem.CollapseBehavior.default

The item uses the default collapsing behavior.

macOS 10.11+

``` source
case `default`
```

## See Also

### Constants

case preferResizingSplitViewWithFixedSiblings

The item’s preference is to keep the other panes at their current size and position onscreen, potentially growing or shrinking the window in the direction to best preserve that.

case preferResizingSiblingsWithFixedSplitView

The item’s preference is to resize the other split panes.

case useConstraints

The item collapses and expands using a constraint animation, with a constraint priority of the item’s holding priority.

