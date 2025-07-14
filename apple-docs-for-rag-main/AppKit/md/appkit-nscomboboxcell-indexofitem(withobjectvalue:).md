

- AppKit
- NSComboBoxCell
-  indexOfItem(withObjectValue:) 

Instance Method

# indexOfItem(withObjectValue:)

Searches the combo box’s internal item list for the given object and returns the matching index number.

macOS

``` source
@MainActor
func indexOfItem(withObjectValue object: Any) -> Int
```

## Parameters 

`object`  

The object for which to return the index.

## Return Value

The lowest index whose corresponding value is equal to `anObject`. Objects are considered equal if they have the same id or if `isEqual:` returns true. If none of the objects in the combo box’s internal item list is equal to `anObject`, indexOfItem(withObjectValue:) returns `NSNotFound`.

## Discussion

This method logs a warning if usesDataSource is true.

## See Also

### Related Documentation

func selectItem(withObjectValue: Any?)

Selects the first pop-up list item that corresponds to the specified object.

### Manipulating the Displayed List

func itemObjectValue(at: Int) -> Any

Returns the object located at the specified location in the internal item list.

func noteNumberOfItemsChanged()

Informs the combo box that the number of items in its data source has changed.

func reloadData()

Marks the combo box as needing redisplay, so that it will reload the data for visible pop-up items and draw the new values.

func scrollItemAtIndexToTop(Int)

Scrolls the combo box’s pop-up list vertically so that the item at the given index is as close to the top as possible.

func scrollItemAtIndexToVisible(Int)

Scrolls the combo box’s pop-up list vertically so that the item at the given index is visible.

