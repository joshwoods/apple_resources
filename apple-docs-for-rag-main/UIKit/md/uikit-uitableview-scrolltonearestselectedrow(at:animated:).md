

- UIKit
- UITableView
-  scrollToNearestSelectedRow(at:animated:) 

Instance Method

# scrollToNearestSelectedRow(at:animated:)

Scrolls the table view so that the selected row nearest to a specified position in the table view is at that position.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func scrollToNearestSelectedRow(
    at scrollPosition: UITableView.ScrollPosition,
    animated: Bool
)
```

## Parameters 

`scrollPosition`  

A constant that identifies a relative position in the table view (top, middle, bottom) for the row when scrolling concludes. See UITableView.ScrollPosition for a descriptions of valid constants.

`animated`  

true if you want to animate the change in position; false if it should be immediate.

## See Also

### Scrolling the table view

func scrollToRow(at: IndexPath, at: UITableView.ScrollPosition, animated: Bool)

Scrolls through the table view until a row that an index path identifies is at a particular location on the screen.

enum ScrollPosition

The position in the table view (top, middle, bottom) to scroll a specified row to.

