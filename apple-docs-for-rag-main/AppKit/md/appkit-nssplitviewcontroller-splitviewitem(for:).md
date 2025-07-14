

- AppKit
- NSSplitViewController
-  splitViewItem(for:) 

Instance Method

# splitViewItem(for:)

Returns the corresponding split view item for the specified child view controller of the split view controller.

macOS 10.10+

``` source
@MainActor
func splitViewItem(for viewController: NSViewController) -> NSSplitViewItem?
```

## Parameters 

`viewController`  

The child view controller with the corresponding split view item you want.

## Return Value

The corresponding split view item, or `nil` if `viewController` isn’t a child of the split view controller.

## See Also

### Configuring and Managing a Split View Controller

var splitView: NSSplitView

The split view that the split view controller manages.

var splitViewItems: [NSSplitViewItem]

The array of split view items that correspond to the split view controller’s child view controllers.

class NSSplitViewItem

An item in a split view controller.

