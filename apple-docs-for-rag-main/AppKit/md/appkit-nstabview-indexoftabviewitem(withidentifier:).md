

- AppKit
- NSTabView
-  indexOfTabViewItem(withIdentifier:) 

Instance Method

# indexOfTabViewItem(withIdentifier:)

Returns the index of the item that matches the specified identifier or `NSNotFound` if the item is not found.

macOS

``` source
@MainActor
func indexOfTabViewItem(withIdentifier identifier: Any) -> Int
```

## Parameters 

`identifier`  

The identifier of a tab view item.

## Return Value

The zero-based index of the tab view item corresponding to `identifier`, or `NSNotFound` if the item is not found.

## Discussion

The returned index is zero-based.

## See Also

### Related Documentation

func insertTabViewItem(NSTabViewItem, at: Int)

Inserts the specified item into the tab view’s array of tab view items at the specified index.

### Accessing Tabs

func indexOfTabViewItem(NSTabViewItem) -> Int

Returns the index of the specified item in the tab view.

var numberOfTabViewItems: Int

The number of items in the tab view’s array of tab view items.

func tabViewItem(at: Int) -> NSTabViewItem

Returns the tab view item at `index` in the tab view’s array of items.

var tabViewItems: [NSTabViewItem]

The tab view’s array of tab view items.

