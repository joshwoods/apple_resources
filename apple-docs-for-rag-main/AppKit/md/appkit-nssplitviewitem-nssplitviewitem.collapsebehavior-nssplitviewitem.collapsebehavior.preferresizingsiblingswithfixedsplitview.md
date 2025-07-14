

- AppKit
- NSSplitViewItem
- NSSplitViewItem.CollapseBehavior
-  NSSplitViewItem.CollapseBehavior.preferResizingSiblingsWithFixedSplitView 

Case

# NSSplitViewItem.CollapseBehavior.preferResizingSiblingsWithFixedSplitView

The item’s preference is to resize the other split panes.

macOS 10.11+

``` source
case preferResizingSiblingsWithFixedSplitView
```

## Discussion

The split view item breaks this preference if it can’t fully expand without causing the other split panes to resize below their minimum size threshold.

## See Also

### Constants

case `default`

The item uses the default collapsing behavior.

case preferResizingSplitViewWithFixedSiblings

The item’s preference is to keep the other panes at their current size and position onscreen, potentially growing or shrinking the window in the direction to best preserve that.

case useConstraints

The item collapses and expands using a constraint animation, with a constraint priority of the item’s holding priority.

