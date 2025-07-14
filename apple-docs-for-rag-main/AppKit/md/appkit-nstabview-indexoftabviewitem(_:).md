

- AppKit
- NSTabView
-  indexOfTabViewItem(\_:) 

Instance Method

# indexOfTabViewItem(\_:)

Returns the index of the specified item in the tab view.

macOS

``` source
@MainActor
func indexOfTabViewItem(_ tabViewItem: NSTabViewItem) -> Int
```

## Parameters 

`tabViewItem`  

The tab view item.

## Return Value

The zero-based index of `tabViewItem`, or `NSNotFound` if the item is not found.

## Discussion

The returned index is zero-based.

## See Also

### Related Documentation

func insertTabViewItem(NSTabViewItem, at: Int)

Inserts the specified item into the tab view’s array of tab view items at the specified index.

### Accessing Tabs

func indexOfTabViewItem(withIdentifier: Any) -> Int

Returns the index of the item that matches the specified identifier or `NSNotFound` if the item is not found.

var numberOfTabViewItems: Int

The number of items in the tab view’s array of tab view items.

func tabViewItem(at: Int) -> NSTabViewItem

Returns the tab view item at `index` in the tab view’s array of items.

var tabViewItems: [NSTabViewItem]

The tab view’s array of tab view items.

