

- AppKit
- NSComboBoxDataSource
-  comboBox(\_:objectValueForItemAt:) 

Instance Method

# comboBox(\_:objectValueForItemAt:)

Returns the object that corresponds to the item at the specified index in the combo box.

macOS

``` source
@MainActor
optional func comboBox(
    _ comboBox: NSComboBox,
    objectValueForItemAt index: Int
) -> Any?
```

## Parameters 

`comboBox`  

The combo box.

`index`  

The index of the item to return.

## Return Value

The object corresponding to the specified index number.

## Discussion

An `NSComboBox` object uses this method to populate the items displayed in its pop-up list.

Important

While this method is marked as `@optional` in the protocol, you must implement this method if you are not providing the data for the combo box using Cocoa bindings.

## See Also

### Related Documentation

Combo Box Programming Topics

### Instance Methods

func comboBox(NSComboBox, completedString: String) -> String?

Returns the first item from the pop-up list that starts with the text the user has typed.

func comboBox(NSComboBox, indexOfItemWithStringValue: String) -> Int

Returns the index of the combo box item matching the specified string.

func numberOfItems(in: NSComboBox) -> Int

Returns the number of items that the data source manages for the combo box.

