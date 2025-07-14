

- AppKit
- NSSplitViewItem
- NSSplitViewItem.CollapseBehavior
-  NSSplitViewItem.CollapseBehavior.preferResizingSplitViewWithFixedSiblings 

Case

# NSSplitViewItem.CollapseBehavior.preferResizingSplitViewWithFixedSiblings

The item’s preference is to keep the other panes at their current size and position onscreen, potentially growing or shrinking the window in the direction to best preserve that.

macOS 10.11+

``` source
case preferResizingSplitViewWithFixedSiblings
```

## Discussion

The split view item breaks this preference in full-screen mode, and to keep the window fully onscreen during resizing.

## See Also

### Constants

case `default`

The item uses the default collapsing behavior.

case preferResizingSiblingsWithFixedSplitView

The item’s preference is to resize the other split panes.

case useConstraints

The item collapses and expands using a constraint animation, with a constraint priority of the item’s holding priority.

