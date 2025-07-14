

- AppKit
- NSComboBox
-  removeItem(at:) 

Instance Method

# removeItem(at:)

Removes the object at the specified location from the receiver’s internal item list.

macOS

``` source
@MainActor
func removeItem(at index: Int)
```

## Parameters 

`index`  

The index of the object to remove. All items beyond `index` are moved up one slot to fill the gap.

## Discussion

The removed object receives a `release` message. This method raises an `NSRangeException` if `index` is beyond the end of the list and logs a warning if the usesDataSource property is true.

## See Also

### Configuring the Combo Box Items

func addItems(withObjectValues: [Any])

Adds multiple objects to the end of the receiver’s internal item list.

func addItem(withObjectValue: Any)

Adds an object to the end of the receiver’s internal item list.

func insertItem(withObjectValue: Any, at: Int)

Inserts an object at the specified location in the receiver’s internal item list.

var objectValues: [Any]

An array of the items from the combo box’s internal list.

func removeAllItems()

Removes all items from the receiver’s internal item list.

func removeItem(withObjectValue: Any)

Removes all occurrences of the given object from the receiver’s internal item list.

var numberOfItems: Int

The total number of items in the pop-up list.

