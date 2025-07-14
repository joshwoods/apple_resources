

- AppKit
- NSPopUpButtonCell
-  removeItem(at:) 

Instance Method

# removeItem(at:)

Removes the item at the specified index.

macOS

``` source
@MainActor
func removeItem(at index: Int)
```

## Parameters 

`index`  

The zero-based index indicating which item to remove. Specifying `0` removes the item at the top of the menu. The index must be valid and non-negative.

## See Also

### Adding and removing items

func addItem(withTitle: String)

Adds an item with the specified title to the end of the menu.

func addItems(withTitles: [String])

Adds multiple items to the end of the menu.

func insertItem(withTitle: String, at: Int)

Inserts an item at the specified position in the menu.

func removeItem(withTitle: String)

Removes the item with the specified title from the menu.

func removeAllItems()

Removes all items in the receiver’s item menu.

