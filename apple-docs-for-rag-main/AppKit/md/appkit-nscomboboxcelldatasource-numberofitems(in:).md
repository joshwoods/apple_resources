

- AppKit
- NSComboBoxCellDataSource
-  numberOfItems(in:) 

Instance Method

# numberOfItems(in:)

Returns the number of items managed for the combo box cell by your data source object.

macOS

``` source
optional func numberOfItems(in comboBoxCell: NSComboBoxCell) -> Int
```

## Parameters 

`comboBoxCell`  

The combo box cell for which your data source manages items.

## Return Value

The number of items your data source object manages.

## Discussion

An `NSComboBoxCell` object uses this method to determine how many items it should display in its pop-up list.

Important

While this method is marked as `@optional` in the protocol, **you must implement this method if you are not providing the data for the combo box using Cocoa bindings**.

## See Also

### Instance Methods

func comboBoxCell(NSComboBoxCell, completedString: String) -> String?

Returns the item from the combo box’s pop-up list that matches the text entered by the user.

func comboBoxCell(NSComboBoxCell, indexOfItemWithStringValue: String) -> Int

Invoked by an `NSComboBoxCell` object to synchronize the pop-up list’s selected item with the text field’s contents.

func comboBoxCell(NSComboBoxCell, objectValueForItemAt: Int) -> Any

Returns the object that corresponds to the item at the given index in the combo box cell.

