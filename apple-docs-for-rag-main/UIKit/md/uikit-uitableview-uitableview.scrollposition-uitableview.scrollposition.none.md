

- UIKit
- UITableView
- UITableView.ScrollPosition
-  UITableView.ScrollPosition.none 

Case

# UITableView.ScrollPosition.none

The table view scrolls the row of interest to be fully visible with a minimum of movement.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
case none
```

## Discussion

If the row is already fully visible, no scrolling occurs. For example, if the row is above the visible area, the behavior is identical to that specified by UITableView.ScrollPosition.top. This is the default.

## See Also

### Constants

case top

The table view scrolls the row of interest to the top of the visible table view.

case middle

The table view scrolls the row of interest to the middle of the visible table view.

case bottom

The table view scrolls the row of interest to the bottom of the visible table view.

