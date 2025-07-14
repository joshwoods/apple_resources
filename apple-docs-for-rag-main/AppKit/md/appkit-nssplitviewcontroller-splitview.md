

- AppKit
- NSSplitViewController
-  splitView 

Instance Property

# splitView

The split view that the split view controller manages.

macOS 10.10+

``` source
@MainActor
var splitView: NSSplitView { get set }
```

## Discussion

This property gives you access to the split view controller’s split view for querying its attributes or customizing it.

By default, a split view arranges its child views vertically from top to bottom. To specify a horizontal (side-by-side) arrangement, implement the isVertical property of the split view object to return true.

Also by default, a split view has a divider style of NSSplitView.DividerStyle.thin, and doesn’t have an autosave name.

Important

Don’t change the delegate property of a split view through the splitView property of a split view controller, and don’t call any methods on the split view object using this property. If you do, the system raises an exception.

To provide a custom split view, set this property at any time before you call `super` in the inherited viewDidLoad() method; that is, before the split view controller’s isViewLoaded property is true.

The split view isn’t always the same object as that in the split view controller’s inherited view property. To access the split view, always use the splitView property.

## See Also

### Configuring and Managing a Split View Controller

func splitViewItem(for: NSViewController) -> NSSplitViewItem?

Returns the corresponding split view item for the specified child view controller of the split view controller.

var splitViewItems: [NSSplitViewItem]

The array of split view items that correspond to the split view controller’s child view controllers.

class NSSplitViewItem

An item in a split view controller.

