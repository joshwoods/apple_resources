

- AppKit
-  NSComboBoxCellDataSource 

Protocol

# NSComboBoxCellDataSource

macOS

``` source
protocol NSComboBoxCellDataSource : NSObjectProtocol
```

## Topics

### Instance Methods

func comboBoxCell(NSComboBoxCell, completedString: String) -> String?

Returns the item from the combo box’s pop-up list that matches the text entered by the user.

func comboBoxCell(NSComboBoxCell, indexOfItemWithStringValue: String) -> Int

Invoked by an `NSComboBoxCell` object to synchronize the pop-up list’s selected item with the text field’s contents.

func comboBoxCell(NSComboBoxCell, objectValueForItemAt: Int) -> Any

Returns the object that corresponds to the item at the given index in the combo box cell.

func numberOfItems(in: NSComboBoxCell) -> Int

Returns the number of items managed for the combo box cell by your data source object.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Cells

class NSComboBoxCell

The user interface of a combo box.

