

- AppKit
- NSComboBox
-  itemObjectValue(at:) 

Instance Method

# itemObjectValue(at:)

Returns the object located at the given index within the receiver’s internal item list.

macOS

``` source
@MainActor
func itemObjectValue(at index: Int) -> Any
```

## Parameters 

`index`  

The index of the object to retrieve. If `index` is beyond the end of the list, an `NSRangeException` is raised.

## Return Value

The object located at the specified index in the internal item list.

## Discussion

This method logs a warning if the usesDataSource property is true.

## See Also

### Related Documentation

var objectValueOfSelectedItem: Any?

The object corresponding to the last item selected from the pop-up list.

### Manipulating the Displayed List

func indexOfItem(withObjectValue: Any) -> Int

Searches the receiver’s internal item list for the specified object and returns the lowest matching index.

func noteNumberOfItemsChanged()

Informs the receiver that the number of items in its data source has changed.

func reloadData()

Marks the receiver as needing redisplay, so that it will reload the data for visible pop-up items and draw the new values.

func scrollItemAtIndexToTop(Int)

Scrolls the receiver’s pop-up list vertically so that the item at the specified index is as close to the top as possible.

func scrollItemAtIndexToVisible(Int)

Scrolls the receiver’s pop-up list vertically so that the item at the specified index is visible.

