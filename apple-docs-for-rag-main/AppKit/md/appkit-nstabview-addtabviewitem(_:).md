

- AppKit
- NSTabView
-  addTabViewItem(\_:) 

Instance Method

# addTabViewItem(\_:)

Adds the specified tab item.

macOS

``` source
@MainActor
func addTabViewItem(_ tabViewItem: NSTabViewItem)
```

## Parameters 

`tabViewItem`  

The tab view item to be added.

## Discussion

The item is added at the end of the array of tab items, so the new tab appears on the right side of the view. If the delegate supports it, it invokes the delegate’s tabViewDidChangeNumberOfTabViewItems(_:) method.

## See Also

### Related Documentation

Tab View Programming Topics

func tabViewItem(at: Int) -> NSTabViewItem

Returns the tab view item at `index` in the tab view’s array of items.

var numberOfTabViewItems: Int

The number of items in the tab view’s array of tab view items.

var tabViewItems: [NSTabViewItem]

The tab view’s array of tab view items.

### Adding and Removing Tabs

func insertTabViewItem(NSTabViewItem, at: Int)

Inserts the specified item into the tab view’s array of tab view items at the specified index.

func removeTabViewItem(NSTabViewItem)

Removes the specified item from the tab view’s array of tab view items.

