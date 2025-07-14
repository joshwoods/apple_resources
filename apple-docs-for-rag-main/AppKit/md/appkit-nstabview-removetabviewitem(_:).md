

- AppKit
- NSTabView
-  removeTabViewItem(\_:) 

Instance Method

# removeTabViewItem(\_:)

Removes the specified item from the tab view’s array of tab view items.

macOS

``` source
@MainActor
func removeTabViewItem(_ tabViewItem: NSTabViewItem)
```

## Parameters 

`tabViewItem`  

The tab view item to be removed.

## Discussion

If there is a delegate and the delegate supports it, sends the delegate the tabViewDidChangeNumberOfTabViewItems(_:) message.

## See Also

### Related Documentation

var tabViewItems: [NSTabViewItem]

The tab view’s array of tab view items.

### Adding and Removing Tabs

func addTabViewItem(NSTabViewItem)

Adds the specified tab item.

func insertTabViewItem(NSTabViewItem, at: Int)

Inserts the specified item into the tab view’s array of tab view items at the specified index.

