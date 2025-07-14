

- AppKit
- NSTabView
-  selectTabViewItem(at:) 

Instance Method

# selectTabViewItem(at:)

Selects the tab view item specified by `index`.

macOS

``` source
@MainActor
func selectTabViewItem(at index: Int)
```

## Parameters 

`index`  

The index of the tab item to selected.

## Discussion

The `index` parameter is base 0. If there is a delegate and the delegate supports it, sends the delegate the tabView(_:shouldSelect:) message.

## See Also

### Related Documentation

func insertTabViewItem(NSTabViewItem, at: Int)

Inserts the specified item into the tab view’s array of tab view items at the specified index.

### Selecting a Tab

func selectFirstTabViewItem(Any?)

This action method selects the first tab view item.

func selectLastTabViewItem(Any?)

This action method selects the last tab view item.

func selectNextTabViewItem(Any?)

This action method selects the next tab view item in the sequence.

func selectPreviousTabViewItem(Any?)

This action method selects the previous tab view item in the sequence.

func selectTabViewItem(NSTabViewItem?)

Selects the specified tab view item.

func selectTabViewItem(withIdentifier: Any)

Selects the tab view item specified by `identifier`.

var selectedTabViewItem: NSTabViewItem?

The tab view item for the currently selected tab.

func takeSelectedTabViewItemFromSender(Any?)

Sets the selected tab view item to the selected item obtained from the sender.

