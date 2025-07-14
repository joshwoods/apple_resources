

- AppKit
- NSComboBox
-  removeItem(withObjectValue:) 

Instance Method

# removeItem(withObjectValue:)

Removes all occurrences of the given object from the receiver’s internal item list.

macOS

``` source
@MainActor
func removeItem(withObjectValue object: Any)
```

## Parameters 

`object`  

The object to remove from the internal item list. Objects are considered equal if they have the same id or if `isEqual:` returns true.

## Discussion

This method logs a warning if the usesDataSource property is true.

## See Also

### Related Documentation

func indexOfItem(withObjectValue: Any) -> Int

Searches the receiver’s internal item list for the specified object and returns the lowest matching index.

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

var numberOfItems: Int

The total number of items in the pop-up list.

