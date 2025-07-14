

- AppKit
- NSComboBoxCell
-  insertItem(withObjectValue:at:) 

Instance Method

# insertItem(withObjectValue:at:)

Inserts an object at the specified location in the internal item list.

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

The object to add to the combo box’s internal item list.

`index`  

The index at which to add the specified object. The previous item at `index`—along with all following items—is shifted down one slot to make room.

## Discussion

This method logs a warning if usesDataSource is true.

## See Also

### Working with an Internal List

func addItems(withObjectValues: [Any])

Adds multiple objects to the internal item list.

func addItem(withObjectValue: Any)

Adds the specified object to the internal item list.

var objectValues: [Any]

The combo box’s internal item list in an array.

func removeAllItems()

Removes all items from the combo box’s internal item list.

func removeItem(at: Int)

Removes the object at the specified location from the combo box’s internal item list.

func removeItem(withObjectValue: Any)

Removes all occurrences of the specified object from the combo box’s internal item list.

var numberOfItems: Int

The total number of items in the pop-up list.

