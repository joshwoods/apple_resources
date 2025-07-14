

- AppKit
- NSTabViewController
-  selectedTabViewItemIndex 

Instance Property

# selectedTabViewItemIndex

The index of the selected tab.

macOS 10.10+

``` source
@MainActor
var selectedTabViewItemIndex: Int { get set }
```

## Discussion

Use this property to get and set the selected tab. The property is key-value coding compliant and can be the target of bindings.

## See Also

### Managing Tab View Items

var tabViewItems: [NSTabViewItem]

The array of tab view items used to manage each of the child view controllers.

func tabViewItem(for: NSViewController) -> NSTabViewItem?

Returns the tab view item for the specified child view controller.

func addTabViewItem(NSTabViewItem)

Adds the specified tab to the end of the tab view controller’s list of tabs.

func insertTabViewItem(NSTabViewItem, at: Int)

Inserts a tab view into the tab view controller’s list of tabs.

func removeTabViewItem(NSTabViewItem)

Removes the specified tab view item from the tab view controller.

