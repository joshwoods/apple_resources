

- AppKit
- NSPopUpButton
-  removeAllItems() 

Instance Method

# removeAllItems()

Removes all items in the receiver’s item menu.

macOS

``` source
@MainActor
func removeAllItems()
```

## Discussion

After removing the items, this method uses the synchronizeTitleAndSelectedItem() method to refresh the menu.

## See Also

### Related Documentation

var numberOfItems: Int

The number of items in the menu.

### Inserting and deleting items

func addItem(withTitle: String)

Adds an item with the specified title to the end of the menu.

func addItems(withTitles: [String])

Adds multiple items to the end of the menu.

func insertItem(withTitle: String, at: Int)

Inserts an item at the specified position in the menu.

func removeItem(withTitle: String)

Removes the item with the specified title from the menu.

func removeItem(at: Int)

Removes the item at the specified index.

