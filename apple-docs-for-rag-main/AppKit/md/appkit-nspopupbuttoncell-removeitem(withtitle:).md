

- AppKit
- NSPopUpButtonCell
-  removeItem(withTitle:) 

Instance Method

# removeItem(withTitle:)

Removes the item with the specified title from the menu.

macOS

``` source
@MainActor
func removeItem(withTitle title: String)
```

## Parameters 

`title`  

The title of the item you want to remove. If no menu item exists with the specified title, this method triggers an assertion.

## See Also

### Adding and removing items

func addItem(withTitle: String)

Adds an item with the specified title to the end of the menu.

func addItems(withTitles: [String])

Adds multiple items to the end of the menu.

func insertItem(withTitle: String, at: Int)

Inserts an item at the specified position in the menu.

func removeItem(at: Int)

Removes the item at the specified index.

func removeAllItems()

Removes all items in the receiver’s item menu.

