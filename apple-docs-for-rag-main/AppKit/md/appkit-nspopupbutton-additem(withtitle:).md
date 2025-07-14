

- AppKit
- NSPopUpButton
-  addItem(withTitle:) 

Instance Method

# addItem(withTitle:)

Adds an item with the specified title to the end of the menu.

macOS

``` source
@MainActor
func addItem(withTitle title: String)
```

## Parameters 

`title`  

The title of the menu-item entry. If an item with the same title already exists in the menu, the existing item is removed and the new one is added.

## Discussion

If you want to move an item, it’s better to invoke removeItem(withTitle:) explicitly and then send this method. After adding the item, this method calls the synchronizeTitleAndSelectedItem() method to make sure the item being displayed matches the currently selected item.

Since this method searches for duplicate items, it should not be used if you are adding an item to an already populated menu with more than a few hundred items. Add items directly to the receiver’s menu instead.

## See Also

### Related Documentation

func setTitle(String)

Sets the string displayed in the receiver when the user isn’t pressing the mouse button.

### Inserting and deleting items

func addItems(withTitles: [String])

Adds multiple items to the end of the menu.

func insertItem(withTitle: String, at: Int)

Inserts an item at the specified position in the menu.

func removeAllItems()

Removes all items in the receiver’s item menu.

func removeItem(withTitle: String)

Removes the item with the specified title from the menu.

func removeItem(at: Int)

Removes the item at the specified index.

