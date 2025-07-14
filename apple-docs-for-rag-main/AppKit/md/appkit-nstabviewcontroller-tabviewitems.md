

- AppKit
- NSTabViewController
-  tabViewItems 

Instance Property

# tabViewItems

The array of tab view items used to manage each of the child view controllers.

macOS 10.10+

``` source
@MainActor
var tabViewItems: [NSTabViewItem] { get set }
```

## Discussion

This property contains an array of NSTabViewItem objects. Each tab view item contains information about a tab in the tab view interface, including the child view controller that manages the tab’s contents.

Assigning a new array to this property updates the set of tabs displayed by the tab view controller.

## See Also

### Managing Tab View Items

func tabViewItem(for: NSViewController) -> NSTabViewItem?

Returns the tab view item for the specified child view controller.

func addTabViewItem(NSTabViewItem)

Adds the specified tab to the end of the tab view controller’s list of tabs.

func insertTabViewItem(NSTabViewItem, at: Int)

Inserts a tab view into the tab view controller’s list of tabs.

func removeTabViewItem(NSTabViewItem)

Removes the specified tab view item from the tab view controller.

var selectedTabViewItemIndex: Int

The index of the selected tab.

