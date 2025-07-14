

- AppKit
- NSComboBoxCellDataSource
-  comboBoxCell(\_:objectValueForItemAt:) 

Instance Method

# comboBoxCell(\_:objectValueForItemAt:)

Returns the object that corresponds to the item at the given index in the combo box cell.

macOS

``` source
optional func comboBoxCell(
    _ comboBoxCell: NSComboBoxCell,
    objectValueForItemAt index: Int
) -> Any
```

## Parameters 

`comboBoxCell`  

The combo box cell for which to return the item.

`index`  

The index of the item to return.

## Return Value

The object corresponding to the item at the specified index in the given combo box cell.

## Discussion

An `NSComboBoxCell` object uses this method to populate the items displayed in its pop-up list.

Important

While this method is marked as `@optional` in the protocol, **you must implement this method if you are not providing the data for the combo box using using Cocoa bindings**.

## See Also

### Related Documentation

Combo Box Programming Topics

### Instance Methods

func comboBoxCell(NSComboBoxCell, completedString: String) -> String?

Returns the item from the combo box’s pop-up list that matches the text entered by the user.

func comboBoxCell(NSComboBoxCell, indexOfItemWithStringValue: String) -> Int

Invoked by an `NSComboBoxCell` object to synchronize the pop-up list’s selected item with the text field’s contents.

func numberOfItems(in: NSComboBoxCell) -> Int

Returns the number of items managed for the combo box cell by your data source object.

