

- AppKit
- NSTabView
-  selectLastTabViewItem(\_:) 

Instance Method

# selectLastTabViewItem(\_:)

This action method selects the last tab view item.

macOS

``` source
@MainActor
func selectLastTabViewItem(_ sender: Any?)
```

## Parameters 

`sender`  

Typically the object that sent invoked the message.

## See Also

### Selecting a Tab

func selectFirstTabViewItem(Any?)

This action method selects the first tab view item.

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

var selectedTabViewItem: NSTabViewItem?

The tab view item for the currently selected tab.

func takeSelectedTabViewItemFromSender(Any?)

Sets the selected tab view item to the selected item obtained from the sender.

