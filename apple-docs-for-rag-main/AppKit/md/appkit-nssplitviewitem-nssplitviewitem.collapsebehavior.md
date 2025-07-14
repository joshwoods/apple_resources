

- AppKit
- NSSplitViewItem
-  NSSplitViewItem.CollapseBehavior 

Enumeration

# NSSplitViewItem.CollapseBehavior

Constants that describe the split view item’s collapsing behavior.

macOS 10.11+

``` source
enum CollapseBehavior
```

## Topics

### Constants

case `default`

The item uses the default collapsing behavior.

case preferResizingSplitViewWithFixedSiblings

The item’s preference is to keep the other panes at their current size and position onscreen, potentially growing or shrinking the window in the direction to best preserve that.

case preferResizingSiblingsWithFixedSplitView

The item’s preference is to resize the other split panes.

case useConstraints

The item collapses and expands using a constraint animation, with a constraint priority of the item’s holding priority.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Collapsing and Expanding the Item

var isCollapsed: Bool

A Boolean value that determines whether the child view controller that corresponds to the split view item is in a collapsed state in the split view controller.

var canCollapse: Bool

A Boolean value that determines whether a user interaction can collapse the child view controller that corresponds to the split view item.

var collapseBehavior: NSSplitViewItem.CollapseBehavior

The resizing behavior when the split view item toggles its collapsed state.

var isSpringLoaded: Bool

A Boolean value that determines whether the split view item can temporarily expand during a drag.

var canCollapseFromWindowResize: Bool

