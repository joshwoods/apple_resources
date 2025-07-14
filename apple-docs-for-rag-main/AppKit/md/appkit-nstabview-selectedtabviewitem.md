

- AppKit
- NSTabView
-  selectedTabViewItem 

Instance Property

# selectedTabViewItem

The tab view item for the currently selected tab.

macOS

``` source
@MainActor
var selectedTabViewItem: NSTabViewItem? { get }
```

## Discussion

If no item is selected, the value of this property is `nil`.

## See Also

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

func selectTabViewItem(at: Int)

Selects the tab view item specified by `index`.

func selectTabViewItem(withIdentifier: Any)

Selects the tab view item specified by `identifier`.

func takeSelectedTabViewItemFromSender(Any?)

Sets the selected tab view item to the selected item obtained from the sender.

