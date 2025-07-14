

- AppKit
- NSSplitViewItem
-  isSpringLoaded 

Instance Property

# isSpringLoaded

A Boolean value that determines whether the split view item can temporarily expand during a drag.

macOS 10.11+

``` source
var isSpringLoaded: Bool { get set }
```

## Discussion

If the value of this property is true, the split view item can temporarily expand during a drag if the user hovers or force clicks its neighboring divider.

The default value of this property is false.

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

var canCollapseFromWindowResize: Bool

