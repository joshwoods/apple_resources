

- AppKit
- NSComboBoxDataSource
-  comboBox(\_:completedString:) 

Instance Method

# comboBox(\_:completedString:)

Returns the first item from the pop-up list that starts with the text the user has typed.

macOS

``` source
@MainActor
optional func comboBox(
    _ comboBox: NSComboBox,
    completedString string: String
) -> String?
```

## Parameters 

`comboBox`  

The combo box.

`string`  

The string to match against items in the combo box’s pop-up list. This is text that the user has typed.

## Return Value

The first complete string from the items in the combo box’s pop-up list that starts with the string in `uncompletedString`.

## Discussion

An `NSComboBox` object uses this method to perform incremental—or “smart”—searches when the user types into the text field. As the user types in the text field, the receiver uses this method to search for items from the pop-up list that start with what the user has typed. The receiver adds the new text to the end of the field and selects the new text, so when the user types another character, it replaces the new text.

This method is optional. If you don’t implement it, the receiver does not perform incremental searches.

## See Also

### Instance Methods

func comboBox(NSComboBox, indexOfItemWithStringValue: String) -> Int

Returns the index of the combo box item matching the specified string.

func comboBox(NSComboBox, objectValueForItemAt: Int) -> Any?

Returns the object that corresponds to the item at the specified index in the combo box.

func numberOfItems(in: NSComboBox) -> Int

Returns the number of items that the data source manages for the combo box.

