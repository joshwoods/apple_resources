

- AppKit
- NSTabView
-  numberOfTabViewItems 

Instance Property

# numberOfTabViewItems

The number of items in the tab view’s array of tab view items.

macOS

``` source
@MainActor
var numberOfTabViewItems: Int { get }
```

## Discussion

The default value of this property is 0.

## See Also

### Accessing Tabs

func indexOfTabViewItem(NSTabViewItem) -> Int

Returns the index of the specified item in the tab view.

func indexOfTabViewItem(withIdentifier: Any) -> Int

Returns the index of the item that matches the specified identifier or `NSNotFound` if the item is not found.

func tabViewItem(at: Int) -> NSTabViewItem

Returns the tab view item at `index` in the tab view’s array of items.

var tabViewItems: [NSTabViewItem]

The tab view’s array of tab view items.

