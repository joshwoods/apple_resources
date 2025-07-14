

- UIKit
- UITableViewDelegate
-  tableView(\_:didEndDisplaying:forRowAt:) 

Instance Method

# tableView(\_:didEndDisplaying:forRowAt:)

Tells the delegate that the specified cell was removed from the table.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    didEndDisplaying cell: UITableViewCell,
    forRowAt indexPath: IndexPath
)
```

## Parameters 

`tableView`  

The table view that removed the view.

`cell`  

The cell that was removed.

`indexPath`  

The index path of the cell.

## Discussion

Use this method to detect when a cell is removed from a table view, as opposed to monitoring the view itself to see when it appears or disappears.

## See Also

### Tracking the removal of views

func tableView(UITableView, didEndDisplayingHeaderView: UIView, forSection: Int)

Tells the delegate that the specified header view was removed from the table.

func tableView(UITableView, didEndDisplayingFooterView: UIView, forSection: Int)

Tells the delegate that the specified footer view was removed from the table.

