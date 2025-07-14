

- AppKit
- NSPopUpButtonCell
-  addItems(withTitles:) 

Instance Method

# addItems(withTitles:)

Adds multiple items to the end of the menu.

macOS

``` source
@MainActor
func addItems(withTitles itemTitles: [String])
```

## Parameters 

`itemTitles`  

An array of NSString objects containing the titles of the items you want to add. Each string in the array should be unique. If an item with the same title already exists in the menu, the existing item is removed and the new one is added.

## Discussion

The new menu items use the pop-up button’s default action and target, but you can change these using the setAction: and setTarget: methods of the corresponding NSMenuItem object.

If you want to move an item, it’s better to invoke removeItem(withTitle:) explicitly and then call this method. After adding the items, this method uses the synchronizeTitleAndSelectedItem() method to make sure the item being displayed matches the currently selected item.

Because this method searches for duplicate items, it should not be used if you are adding items to an already populated menu with more than a few hundred items. In a situation like this, add items directly to the receiver’s menu instead.

## See Also

### Adding and removing items

func addItem(withTitle: String)

Adds an item with the specified title to the end of the menu.

func insertItem(withTitle: String, at: Int)

Inserts an item at the specified position in the menu.

func removeItem(withTitle: String)

Removes the item with the specified title from the menu.

func removeItem(at: Int)

Removes the item at the specified index.

func removeAllItems()

Removes all items in the receiver’s item menu.

