

- AppKit
- NSTabViewController
-  addTabViewItem(\_:) 

Instance Method

# addTabViewItem(\_:)

Adds the specified tab to the end of the tab view controller’s list of tabs.

macOS 10.10+

``` source
@MainActor
func addTabViewItem(_ tabViewItem: NSTabViewItem)
```

## Parameters 

`tabViewItem`  

The tab view item to add. The tab view item must have an associated view controller. If this parameter is `nil` or if the tab view item does not have a view controller, this method raises an exception.

## Discussion

Use this method to add new tabs to a tab view controller. This method adds the tab’s associated view controller as a child of the tab view controller, so you do not need to call the addChild(_:) method directly. The view for the new view controller is not loaded until its corresponding tab is selected by the user.

If you override this method, you must call `super` at some point in your implementation.

## See Also

### Managing Tab View Items

var tabViewItems: [NSTabViewItem]

The array of tab view items used to manage each of the child view controllers.

func tabViewItem(for: NSViewController) -> NSTabViewItem?

Returns the tab view item for the specified child view controller.

func insertTabViewItem(NSTabViewItem, at: Int)

Inserts a tab view into the tab view controller’s list of tabs.

func removeTabViewItem(NSTabViewItem)

Removes the specified tab view item from the tab view controller.

var selectedTabViewItemIndex: Int

The index of the selected tab.

