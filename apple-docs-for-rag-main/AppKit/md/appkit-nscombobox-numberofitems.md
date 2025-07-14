

- AppKit
- NSComboBox
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

The maximum number of visible items to display in the pop-up list at one time.

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

func removeItem(at: Int)

Removes the object at the specified location from the receiver’s internal item list.

func removeItem(withObjectValue: Any)

Removes all occurrences of the given object from the receiver’s internal item list.

