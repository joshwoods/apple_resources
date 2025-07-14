

- AppKit
- NSComboBox
-  indexOfItem(withObjectValue:) 

Instance Method

# indexOfItem(withObjectValue:)

Searches the receiver’s internal item list for the specified object and returns the lowest matching index.

macOS

``` source
@MainActor
func indexOfItem(withObjectValue object: Any) -> Int
```

## Parameters 

`object`  

The object for which to return the index.

## Return Value

The lowest index in the internal item list whose corresponding value is equal to that of the specified object. Objects are considered equal if they have the same id or if `isEqual:` returns true.

## Discussion

If none of the objects in the receiver’s internal item list are equal to `anObject`, indexOfItem(withObjectValue:) returns `NSNotFound`.

## Discussion

This method logs a warning if the usesDataSource property is true.

## See Also

### Related Documentation

func selectItem(withObjectValue: Any?)

Selects the first pop-up list item that corresponds to the given object.

### Manipulating the Displayed List

func itemObjectValue(at: Int) -> Any

Returns the object located at the given index within the receiver’s internal item list.

func noteNumberOfItemsChanged()

Informs the receiver that the number of items in its data source has changed.

func reloadData()

Marks the receiver as needing redisplay, so that it will reload the data for visible pop-up items and draw the new values.

func scrollItemAtIndexToTop(Int)

Scrolls the receiver’s pop-up list vertically so that the item at the specified index is as close to the top as possible.

func scrollItemAtIndexToVisible(Int)

Scrolls the receiver’s pop-up list vertically so that the item at the specified index is visible.

