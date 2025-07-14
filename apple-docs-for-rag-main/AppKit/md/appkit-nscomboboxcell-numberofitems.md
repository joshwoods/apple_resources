

- AppKit
- NSComboBoxCell
-  numberOfItems 

Instance Property

# numberOfItems

The total number of items in the pop-up list.

macOS

``` source
@MainActor
var numberOfItems: Int { get }
```

## See Also

### Related Documentation

var numberOfVisibleItems: Int

The maximum number of items visible in the pop-up list at any one time.

func numberOfItems(in: NSComboBoxCell) -> Int

Returns the number of items managed for the combo box cell by your data source object.

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

func removeItem(withObjectValue: Any)

Removes all occurrences of the specified object from the combo box’s internal item list.

