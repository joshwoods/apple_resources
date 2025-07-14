

- AppKit
- NSTabView
-  selectTabViewItem(withIdentifier:) 

Instance Method

# selectTabViewItem(withIdentifier:)

Selects the tab view item specified by `identifier`.

macOS

``` source
@MainActor
func selectTabViewItem(withIdentifier identifier: Any)
```

## Parameters 

`identifier`  

The identifier of the tab item to select.

## See Also

### Related Documentation

var identifier: Any?

Sets the receiver’s optional identifier object to `identifier`.

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

var selectedTabViewItem: NSTabViewItem?

The tab view item for the currently selected tab.

func takeSelectedTabViewItemFromSender(Any?)

Sets the selected tab view item to the selected item obtained from the sender.

