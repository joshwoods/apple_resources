

- AppKit
- NSTabView
-  tabViewItem(at:) 

Instance Method

# tabViewItem(at:)

Returns the tab view item at `index` in the tab view’s array of items.

macOS

``` source
@MainActor
func tabViewItem(at index: Int) -> NSTabViewItem
```

## Parameters 

`index`  

The index at which to insert the tab view item. The `index` parameter is zero-based.

## Return Value

The tab view item at the specified index.

## See Also

### Related Documentation

func insertTabViewItem(NSTabViewItem, at: Int)

Inserts the specified item into the tab view’s array of tab view items at the specified index.

### Accessing Tabs

func indexOfTabViewItem(NSTabViewItem) -> Int

Returns the index of the specified item in the tab view.

func indexOfTabViewItem(withIdentifier: Any) -> Int

Returns the index of the item that matches the specified identifier or `NSNotFound` if the item is not found.

var numberOfTabViewItems: Int

The number of items in the tab view’s array of tab view items.

var tabViewItems: [NSTabViewItem]

The tab view’s array of tab view items.

