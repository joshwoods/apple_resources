

- AppKit
- NSComboBox
-  noteNumberOfItemsChanged() 

Instance Method

# noteNumberOfItemsChanged()

Informs the receiver that the number of items in its data source has changed.

macOS

``` source
@MainActor
func noteNumberOfItemsChanged()
```

## Discussion

This method allows the receiver to update the scrollers in its displayed pop-up list without actually reloading data into the receiver. It is particularly useful for a data source that continually receives data in the background over a period of time, in which case the `NSComboBox` can remain responsive to the user while the data is received.

See the NSComboBoxDataSource informal protocol specification for information on the messages an `NSComboBox` sends to its data source.

## See Also

### Manipulating the Displayed List

func indexOfItem(withObjectValue: Any) -> Int

Searches the receiver’s internal item list for the specified object and returns the lowest matching index.

func itemObjectValue(at: Int) -> Any

Returns the object located at the given index within the receiver’s internal item list.

func reloadData()

Marks the receiver as needing redisplay, so that it will reload the data for visible pop-up items and draw the new values.

func scrollItemAtIndexToTop(Int)

Scrolls the receiver’s pop-up list vertically so that the item at the specified index is as close to the top as possible.

func scrollItemAtIndexToVisible(Int)

Scrolls the receiver’s pop-up list vertically so that the item at the specified index is visible.

