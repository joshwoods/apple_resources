

- AppKit
- NSTabViewItem
-  tabView 

Instance Property

# tabView

Returns the parent tab view for the receiver.

macOS

``` source
var tabView: NSTabView? { get }
```

## Discussion

Note that this is the tab view itself, not the view displayed when a user clicks the tab.

A tab view item normally learns about its parent tab view when it is inserted into the view’s array of items. The NSTabView methods addTabViewItem(_:) and insertTabViewItem(_:at:) set the tab view for the added or inserted item.

## See Also

### Related Documentation

var view: NSView?

Sets the view associated with the receiver to `view`.

