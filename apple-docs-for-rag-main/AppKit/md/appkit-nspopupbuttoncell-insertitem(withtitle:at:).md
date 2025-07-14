

- AppKit
- NSPopUpButtonCell
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

The zero-based index at which to insert the item. Specifying `0` inserts the item at the top of the menu.

## Discussion

The value in `index` must represent a valid position in the array. The menu item at `index` and all those that follow it are shifted down one slot to make room for the new menu item.

This method assigns the pop-up button’s default action and target to the new menu item. Use the menu item’s setAction: and setTarget: methods to assign a new action and target.

Because this method searches for duplicate items, it should not be used if you are adding an item to an already populated menu with more than a few hundred items. In a situation like this, add items directly to the button’s menu instead.

## See Also

### Related Documentation

func insert(Any, at: Int)

Inserts a given object into the array’s contents at a given index.

### Adding and removing items

func addItem(withTitle: String)

Adds an item with the specified title to the end of the menu.

func addItems(withTitles: [String])

Adds multiple items to the end of the menu.

func removeItem(withTitle: String)

Removes the item with the specified title from the menu.

func removeItem(at: Int)

Removes the item at the specified index.

func removeAllItems()

Removes all items in the receiver’s item menu.

