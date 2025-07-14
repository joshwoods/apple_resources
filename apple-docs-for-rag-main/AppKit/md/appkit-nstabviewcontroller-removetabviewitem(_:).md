

- AppKit
- NSTabViewController
-  removeTabViewItem(\_:) 

Instance Method

# removeTabViewItem(\_:)

Removes the specified tab view item from the tab view controller.

macOS 10.10+

``` source
@MainActor
func removeTabViewItem(_ tabViewItem: NSTabViewItem)
```

## Parameters 

`tabViewItem`  

The tab view item to remove. If this parameter is `nil` or the item does not belong to the tab view controller, this method throws an exception.

## Discussion

Use this method to remove a tab view item from the tab view interface. Removing the item removes the corresponding view controller from the tab view controller’s list of child view controllers. If the removed tab view item is currently selected, the tab view controller selects the next item (or the previous item if there is no next item). Removing the last tab view item sets the selectedTabViewItemIndex property to `-1`.

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

var selectedTabViewItemIndex: Int

The index of the selected tab.

