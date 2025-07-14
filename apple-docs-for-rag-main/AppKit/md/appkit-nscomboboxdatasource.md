

- AppKit
-  NSComboBoxDataSource 

Protocol

# NSComboBoxDataSource

macOS

``` source
protocol NSComboBoxDataSource : NSObjectProtocol
```

## Topics

### Instance Methods

func comboBox(NSComboBox, completedString: String) -> String?

Returns the first item from the pop-up list that starts with the text the user has typed.

func comboBox(NSComboBox, indexOfItemWithStringValue: String) -> Int

Returns the index of the combo box item matching the specified string.

func comboBox(NSComboBox, objectValueForItemAt: Int) -> Any?

Returns the object that corresponds to the item at the specified index in the combo box.

func numberOfItems(in: NSComboBox) -> Int

Returns the number of items that the data source manages for the combo box.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Management

protocol NSComboBoxDelegate

A set of optional methods implemented by delegates of combo box objects.

