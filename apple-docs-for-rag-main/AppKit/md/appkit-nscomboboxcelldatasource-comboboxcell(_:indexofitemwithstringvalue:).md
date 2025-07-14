

- AppKit
- NSComboBoxCellDataSource
-  comboBoxCell(\_:indexOfItemWithStringValue:) 

Instance Method

# comboBoxCell(\_:indexOfItemWithStringValue:)

Invoked by an `NSComboBoxCell` object to synchronize the pop-up list’s selected item with the text field’s contents.

macOS

``` source
optional func comboBoxCell(
    _ comboBoxCell: NSComboBoxCell,
    indexOfItemWithStringValue string: String
) -> Int
```

## Parameters 

`comboBoxCell`  

The combo box cell.

`string`  

The string to match. If comboBoxCell(_:completedString:) is implemented, `aString` is the string returned by that method. Otherwise, `aString` is the text that the user has typed.

## Return Value

The index for the pop-up list item matching `aString`, or `NSNotFound` if no item matches.

## Discussion

If you don’t implement this method, the receiver does not synchronize the pop-up list’s selected item with the text field’s contents.

## See Also

### Instance Methods

func comboBoxCell(NSComboBoxCell, completedString: String) -> String?

Returns the item from the combo box’s pop-up list that matches the text entered by the user.

func comboBoxCell(NSComboBoxCell, objectValueForItemAt: Int) -> Any

Returns the object that corresponds to the item at the given index in the combo box cell.

func numberOfItems(in: NSComboBoxCell) -> Int

Returns the number of items managed for the combo box cell by your data source object.

