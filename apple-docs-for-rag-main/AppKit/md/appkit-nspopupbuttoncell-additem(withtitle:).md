

- AppKit
- NSPopUpButtonCell
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

The title of the new menu item. If an item with the same title already exists in the menu, the existing item is removed and the new one is added.

## Discussion

The menu item uses the pop-up button’s default action and target, but you can change these using the setAction: and setTarget: methods of the corresponding NSMenuItem object.

Because this method searches for duplicate items, it should not be used if you are adding an item to an already populated menu with more than a few hundred items. In a situation like this, add items directly to the button’s menu instead.

## See Also

### Adding and removing items

func addItems(withTitles: [String])

Adds multiple items to the end of the menu.

func insertItem(withTitle: String, at: Int)

Inserts an item at the specified position in the menu.

func removeItem(withTitle: String)

Removes the item with the specified title from the menu.

func removeItem(at: Int)

Removes the item at the specified index.

func removeAllItems()

Removes all items in the receiver’s item menu.

