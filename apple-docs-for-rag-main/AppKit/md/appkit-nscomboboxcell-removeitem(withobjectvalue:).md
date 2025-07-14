

- AppKit
- NSComboBoxCell
-  removeItem(withObjectValue:) 

Instance Method

# removeItem(withObjectValue:)

Removes all occurrences of the specified object from the combo box’s internal item list.

macOS

``` source
@MainActor
func removeItem(withObjectValue object: Any)
```

## Parameters 

`object`  

The object to remove from the combo box’s internal item list. Objects are considered equal if they have the same id or if `isEqual:` returns true.

## Discussion

This method logs a warning if usesDataSource is true.

## See Also

### Related Documentation

func indexOfItem(withObjectValue: Any) -> Int

Searches the combo box’s internal item list for the given object and returns the matching index number.

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

func removeItem(at: Int)

Removes the object at the specified location from the combo box’s internal item list.

var numberOfItems: Int

The total number of items in the pop-up list.

