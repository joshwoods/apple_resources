

- AppKit
- NSTabView
-  insertTabViewItem(\_:at:) 

Instance Method

# insertTabViewItem(\_:at:)

Inserts the specified item into the tab view’s array of tab view items at the specified index.

macOS

``` source
@MainActor
func insertTabViewItem(
    _ tabViewItem: NSTabViewItem,
    at index: Int
)
```

## Parameters 

`tabViewItem`  

The tab view item to be added.

`index`  

The index at which to insert the tab view item. The `index` parameter is zero-based.

## Discussion

If there is a delegate and the delegate supports it, sends the delegate the tabViewDidChangeNumberOfTabViewItems(_:) message.

## See Also

### Related Documentation

func indexOfTabViewItem(withIdentifier: Any) -> Int

Returns the index of the item that matches the specified identifier or `NSNotFound` if the item is not found.

func tabViewItem(at: Int) -> NSTabViewItem

Returns the tab view item at `index` in the tab view’s array of items.

var numberOfTabViewItems: Int

The number of items in the tab view’s array of tab view items.

func indexOfTabViewItem(NSTabViewItem) -> Int

Returns the index of the specified item in the tab view.

### Adding and Removing Tabs

func addTabViewItem(NSTabViewItem)

Adds the specified tab item.

func removeTabViewItem(NSTabViewItem)

Removes the specified item from the tab view’s array of tab view items.

