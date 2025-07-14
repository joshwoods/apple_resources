

- AppKit
- NSComboBoxCell
-  removeItem(at:) 

Instance Method

# removeItem(at:)

Removes the object at the specified location from the combo box’s internal item list.

macOS

``` source
@MainActor
func removeItem(at index: Int)
```

## Parameters 

`index`  

The index of the object to remove from the combo box’s internal item list. All items beyond `index` are moved up one slot to fill the gap.

## Discussion

The removed object receives a `release` message. This method raises an `NSRangeException` if `index` is beyond the end of the list and logs a warning if usesDataSource is true.

## See Also

### Working with an Internal List

func addItems(withObjectValues: [Any])

Adds multiple objects to the internal item list.

func addItem(withObjectValue: Any)

Adds the specified object to the internal item list.

func insertItem(withObjectValue: Any, at: Int)

Inserts an object at the specified location in the internal item list.

var objectValues: [Any]

The combo box’s internal item list in an array.

func removeAllItems()

Removes all items from the combo box’s internal item list.

func removeItem(withObjectValue: Any)

Removes all occurrences of the specified object from the combo box’s internal item list.

var numberOfItems: Int

The total number of items in the pop-up list.

