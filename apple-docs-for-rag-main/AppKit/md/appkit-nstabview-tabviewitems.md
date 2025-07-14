

- AppKit
- NSTabView
-  tabViewItems 

Instance Property

# tabViewItems

The tab view’s array of tab view items.

macOS

``` source
@MainActor
var tabViewItems: [NSTabViewItem] { get set }
```

## Discussion

A tab view keeps an array containing one tab view item for each tab in the view. The default value of this property is an empty array.

## See Also

### Accessing Tabs

func indexOfTabViewItem(NSTabViewItem) -> Int

Returns the index of the specified item in the tab view.

func indexOfTabViewItem(withIdentifier: Any) -> Int

Returns the index of the item that matches the specified identifier or `NSNotFound` if the item is not found.

var numberOfTabViewItems: Int

The number of items in the tab view’s array of tab view items.

func tabViewItem(at: Int) -> NSTabViewItem

Returns the tab view item at `index` in the tab view’s array of items.

