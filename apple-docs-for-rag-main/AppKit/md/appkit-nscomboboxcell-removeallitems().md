

- AppKit
- NSComboBoxCell
-  removeAllItems() 

Instance Method

# removeAllItems()

Removes all items from the combo box’s internal item list.

macOS

``` source
@MainActor
func removeAllItems()
```

## Discussion

This method logs a warning if usesDataSource is true.

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

func removeItem(at: Int)

Removes the object at the specified location from the combo box’s internal item list.

func removeItem(withObjectValue: Any)

Removes all occurrences of the specified object from the combo box’s internal item list.

var numberOfItems: Int

The total number of items in the pop-up list.

