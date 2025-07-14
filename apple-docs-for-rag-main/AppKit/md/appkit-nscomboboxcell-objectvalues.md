

- AppKit
- NSComboBoxCell
-  objectValues 

Instance Property

# objectValues

The combo box’s internal item list in an array.

macOS

``` source
@MainActor
var objectValues: [Any] { get }
```

## Discussion

Accessing this property logs a warning if usesDataSource is true.

## See Also

### Working with an Internal List

func addItems(withObjectValues: [Any])

Adds multiple objects to the internal item list.

func addItem(withObjectValue: Any)

Adds the specified object to the internal item list.

func insertItem(withObjectValue: Any, at: Int)

Inserts an object at the specified location in the internal item list.

func removeAllItems()

Removes all items from the combo box’s internal item list.

func removeItem(at: Int)

Removes the object at the specified location from the combo box’s internal item list.

func removeItem(withObjectValue: Any)

Removes all occurrences of the specified object from the combo box’s internal item list.

var numberOfItems: Int

The total number of items in the pop-up list.

