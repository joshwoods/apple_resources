

- AppKit
- NSTabViewController
-  tabViewItem(for:) 

Instance Method

# tabViewItem(for:)

Returns the tab view item for the specified child view controller.

macOS 10.10+

``` source
@MainActor
func tabViewItem(for viewController: NSViewController) -> NSTabViewItem?
```

## Parameters 

`viewController`  

The child view controller whose tab view item you want.

## Return Value

The tab view item associated with the view controller or `nil` if the view controller is not managed by the tab view controller.

## Discussion

This method is a convenient way to map a tab view item to a newly added child view controller. When you add child view controllers using the addChild(_:) method, the tab view automatically controller creates a new tab view item. Use this method to fetch that tab view item and configure it.

## See Also

### Managing Tab View Items

var tabViewItems: [NSTabViewItem]

The array of tab view items used to manage each of the child view controllers.

func addTabViewItem(NSTabViewItem)

Adds the specified tab to the end of the tab view controller’s list of tabs.

func insertTabViewItem(NSTabViewItem, at: Int)

Inserts a tab view into the tab view controller’s list of tabs.

func removeTabViewItem(NSTabViewItem)

Removes the specified tab view item from the tab view controller.

var selectedTabViewItemIndex: Int

The index of the selected tab.

