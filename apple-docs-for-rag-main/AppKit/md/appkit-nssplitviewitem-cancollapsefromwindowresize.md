

- AppKit
- NSSplitViewItem
-  canCollapseFromWindowResize 

Instance Property

# canCollapseFromWindowResize

macOS 10.14+

``` source
var canCollapseFromWindowResize: Bool { get set }
```

## See Also

### Collapsing and Expanding the Item

var isCollapsed: Bool

A Boolean value that determines whether the child view controller that corresponds to the split view item is in a collapsed state in the split view controller.

var canCollapse: Bool

A Boolean value that determines whether a user interaction can collapse the child view controller that corresponds to the split view item.

var collapseBehavior: NSSplitViewItem.CollapseBehavior

The resizing behavior when the split view item toggles its collapsed state.

enum CollapseBehavior

Constants that describe the split view item’s collapsing behavior.

var isSpringLoaded: Bool

A Boolean value that determines whether the split view item can temporarily expand during a drag.

