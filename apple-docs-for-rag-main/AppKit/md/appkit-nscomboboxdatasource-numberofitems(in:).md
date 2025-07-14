

- AppKit
- NSComboBoxDataSource
-  numberOfItems(in:) 

Instance Method

# numberOfItems(in:)

Returns the number of items that the data source manages for the combo box.

macOS

``` source
@MainActor
optional func numberOfItems(in comboBox: NSComboBox) -> Int
```

## Parameters 

`comboBox`  

The combo box.

## Return Value

The number of items that the data source object manages for the specified combo box.

## Discussion

An `NSComboBox` object uses this method to determine how many items it should display in its pop-up list.

Important

While this method is marked as `@optional` in the protocol, you must implement this method if you are not providing the data for the combo box using Cocoa bindings.

## See Also

### Instance Methods

func comboBox(NSComboBox, completedString: String) -> String?

Returns the first item from the pop-up list that starts with the text the user has typed.

func comboBox(NSComboBox, indexOfItemWithStringValue: String) -> Int

Returns the index of the combo box item matching the specified string.

func comboBox(NSComboBox, objectValueForItemAt: Int) -> Any?

Returns the object that corresponds to the item at the specified index in the combo box.

