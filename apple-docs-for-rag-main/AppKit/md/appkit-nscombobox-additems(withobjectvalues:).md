

- AppKit
- NSComboBox
-  addItems(withObjectValues:) 

Instance Method

# addItems(withObjectValues:)

Adds multiple objects to the end of the receiver’s internal item list.

macOS

``` source
@MainActor
func addItems(withObjectValues objects: [Any])
```

## Parameters 

`objects`  

An array of the objects to add to the internal item list.

## Discussion

This method logs a warning if the usesDataSource property is true.

## See Also

### Configuring the Combo Box Items

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

var numberOfItems: Int

The total number of items in the pop-up list.

