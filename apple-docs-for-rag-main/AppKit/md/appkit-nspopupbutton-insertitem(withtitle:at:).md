

- AppKit
- NSPopUpButton
-  insertItem(withTitle:at:) 

Instance Method

# insertItem(withTitle:at:)

Inserts an item at the specified position in the menu.

macOS

``` source
@MainActor
func insertItem(
    withTitle title: String,
    at index: Int
)
```

## Parameters 

`title`  

The title of the new item. If an item with the same title already exists in the menu, the existing item is removed and the new one is added

`index`  

The zero-based index at which to insert the item. Specifying 0 inserts the item at the top of the menu.

## Discussion

If you want to move an item, it’s better to invoke removeItem(withTitle:) explicitly and then send this method. After adding the item, this method uses the synchronizeTitleAndSelectedItem() method to make sure the item displayed matches the currently selected item.

Since this method searches for duplicate items, it should not be used if you are adding an item to an already populated menu with more than a few hundred items. Add items directly to the receiver’s menu instead.

## See Also

### Related Documentation

func indexOfItem(withTitle: String) -> Int

Returns the index of the item with the specified title.

### Inserting and deleting items

func addItem(withTitle: String)

Adds an item with the specified title to the end of the menu.

func addItems(withTitles: [String])

Adds multiple items to the end of the menu.

func removeAllItems()

Removes all items in the receiver’s item menu.

func removeItem(withTitle: String)

Removes the item with the specified title from the menu.

func removeItem(at: Int)

Removes the item at the specified index.

