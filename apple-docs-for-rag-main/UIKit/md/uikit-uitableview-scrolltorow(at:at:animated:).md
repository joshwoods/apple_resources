

- UIKit
- UITableView
-  scrollToRow(at:at:animated:) 

Instance Method

# scrollToRow(at:at:animated:)

Scrolls through the table view until a row that an index path identifies is at a particular location on the screen.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func scrollToRow(
    at indexPath: IndexPath,
    at scrollPosition: UITableView.ScrollPosition,
    animated: Bool
)
```

## Parameters 

`indexPath`  

An index path that identifies a row in the table view by its row index and its section index.

`NSNotFound` is a valid row index for scrolling to a section with zero rows.

`scrollPosition`  

A constant that identifies a relative position in the table view (top, middle, bottom) for `row` when scrolling concludes. See UITableView.ScrollPosition for descriptions of valid constants.

`animated`  

true if you want to animate the change in position; false if it should be immediate.

## Discussion

Invoking this method doesn’t cause the delegate to receive a scrollViewDidScroll(_:) message, as is normal for programmatically invoked user interface operations.

## See Also

### Scrolling the table view

func scrollToNearestSelectedRow(at: UITableView.ScrollPosition, animated: Bool)

Scrolls the table view so that the selected row nearest to a specified position in the table view is at that position.

enum ScrollPosition

The position in the table view (top, middle, bottom) to scroll a specified row to.

