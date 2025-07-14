

- AppKit
- NSComboBoxCell
-  reloadData() 

Instance Method

# reloadData()

Marks the combo box as needing redisplay, so that it will reload the data for visible pop-up items and draw the new values.

macOS

``` source
@MainActor
func reloadData()
```

## See Also

### Manipulating the Displayed List

func indexOfItem(withObjectValue: Any) -> Int

Searches the combo box’s internal item list for the given object and returns the matching index number.

func itemObjectValue(at: Int) -> Any

Returns the object located at the specified location in the internal item list.

func noteNumberOfItemsChanged()

Informs the combo box that the number of items in its data source has changed.

func scrollItemAtIndexToTop(Int)

Scrolls the combo box’s pop-up list vertically so that the item at the given index is as close to the top as possible.

func scrollItemAtIndexToVisible(Int)

Scrolls the combo box’s pop-up list vertically so that the item at the given index is visible.

