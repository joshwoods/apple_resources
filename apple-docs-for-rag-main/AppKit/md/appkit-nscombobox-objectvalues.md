

- AppKit
- NSComboBox
-  objectValues 

Instance Property

# objectValues

An array of the items from the combo box’s internal list.

macOS

``` source
@MainActor
var objectValues: [Any] { get }
```

## Discussion

The array contains the objects you added or inserted into the combo box, so the type of each object can vary. Accessing this property logs a warning if the usesDataSource property is true.

## See Also

### Configuring the Combo Box Items

func addItems(withObjectValues: [Any])

Adds multiple objects to the end of the receiver’s internal item list.

func addItem(withObjectValue: Any)

Adds an object to the end of the receiver’s internal item list.

func insertItem(withObjectValue: Any, at: Int)

Inserts an object at the specified location in the receiver’s internal item list.

func removeAllItems()

Removes all items from the receiver’s internal item list.

func removeItem(at: Int)

Removes the object at the specified location from the receiver’s internal item list.

func removeItem(withObjectValue: Any)

Removes all occurrences of the given object from the receiver’s internal item list.

var numberOfItems: Int

The total number of items in the pop-up list.

