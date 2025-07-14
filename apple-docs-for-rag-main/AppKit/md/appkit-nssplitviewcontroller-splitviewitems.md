

- AppKit
- NSSplitViewController
-  splitViewItems 

Instance Property

# splitViewItems

The array of split view items that correspond to the split view controller’s child view controllers.

macOS 10.10+

``` source
@MainActor
var splitViewItems: [NSSplitViewItem] { get set }
```

## Discussion

Setting this property implicitly calls the insertSplitViewItem(_:at:) or removeSplitViewItem(_:) method, as appropriate, to add or remove split view items from this array.

If you add a child view controller to the split view controller, the system automatically creates a default split view item for the child view controller and adds it to the splitViewItems array.

If you remove a child view controller, the split view controller removes its corresponding split view item from the splitViewItems array.

## See Also

### Configuring and Managing a Split View Controller

var splitView: NSSplitView

The split view that the split view controller manages.

func splitViewItem(for: NSViewController) -> NSSplitViewItem?

Returns the corresponding split view item for the specified child view controller of the split view controller.

class NSSplitViewItem

An item in a split view controller.

