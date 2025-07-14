

- AppKit
- NSComboBoxCell
-  itemObjectValue(at:) 

Instance Method

# itemObjectValue(at:)

Returns the object located at the specified location in the internal item list.

macOS

``` source
@MainActor
func itemObjectValue(at index: Int) -> Any
```

## Parameters 

`index`  

The index of the object to return. If `index` is beyond the end of the list, an `NSRangeException` is raised.

## Return Value

The object at the given location in the combo box’s internal item list.

## Discussion

This method logs a warning if usesDataSource is true.

## See Also

### Related Documentation

var objectValueOfSelectedItem: Any?

The object corresponding to the last item selected from the pop-up list.

### Manipulating the Displayed List

func indexOfItem(withObjectValue: Any) -> Int

Searches the combo box’s internal item list for the given object and returns the matching index number.

func noteNumberOfItemsChanged()

Informs the combo box that the number of items in its data source has changed.

func reloadData()

Marks the combo box as needing redisplay, so that it will reload the data for visible pop-up items and draw the new values.

func scrollItemAtIndexToTop(Int)

Scrolls the combo box’s pop-up list vertically so that the item at the given index is as close to the top as possible.

func scrollItemAtIndexToVisible(Int)

Scrolls the combo box’s pop-up list vertically so that the item at the given index is visible.

