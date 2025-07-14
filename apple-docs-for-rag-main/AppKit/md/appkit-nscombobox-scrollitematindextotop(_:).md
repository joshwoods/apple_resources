

- AppKit
- NSComboBox
-  scrollItemAtIndexToTop(\_:) 

Instance Method

# scrollItemAtIndexToTop(\_:)

Scrolls the receiver’s pop-up list vertically so that the item at the specified index is as close to the top as possible.

macOS

``` source
@MainActor
func scrollItemAtIndexToTop(_ index: Int)
```

## Parameters 

`index`  

The index of the item to scroll to the top.

## Discussion

The pop-up list need not be displayed at the time this method is invoked.

## See Also

### Manipulating the Displayed List

func indexOfItem(withObjectValue: Any) -> Int

Searches the receiver’s internal item list for the specified object and returns the lowest matching index.

func itemObjectValue(at: Int) -> Any

Returns the object located at the given index within the receiver’s internal item list.

func noteNumberOfItemsChanged()

Informs the receiver that the number of items in its data source has changed.

func reloadData()

Marks the receiver as needing redisplay, so that it will reload the data for visible pop-up items and draw the new values.

func scrollItemAtIndexToVisible(Int)

Scrolls the receiver’s pop-up list vertically so that the item at the specified index is visible.

