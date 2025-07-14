

- AppKit
- NSComboBox
-  insertItem(withObjectValue:at:) 

Instance Method

# insertItem(withObjectValue:at:)

Inserts an object at the specified location in the receiver’s internal item list.

macOS

``` source
@MainActor
func insertItem(
    withObjectValue object: Any,
    at index: Int
)
```

## Parameters 

`object`  

The object to add to the internal item list.

`index`  

The index in the list at which to add the new object. The previous item at `index`—along with all following items—is shifted down one slot to make room

## Discussion

This method logs a warning if the usesDataSource property is true.

## See Also

### Configuring the Combo Box Items

func addItems(withObjectValues: [Any])

Adds multiple objects to the end of the receiver’s internal item list.

func addItem(withObjectValue: Any)

Adds an object to the end of the receiver’s internal item list.

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

