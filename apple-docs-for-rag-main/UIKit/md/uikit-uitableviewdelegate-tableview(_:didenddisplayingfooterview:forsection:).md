

- UIKit
- UITableViewDelegate
-  tableView(\_:didEndDisplayingFooterView:forSection:) 

Instance Method

# tableView(\_:didEndDisplayingFooterView:forSection:)

Tells the delegate that the specified footer view was removed from the table.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    didEndDisplayingFooterView view: UIView,
    forSection section: Int
)
```

## Parameters 

`tableView`  

The table view that removed the view.

`view`  

The footer view that was removed.

`section`  

The index of the section that contained the footer.

## Discussion

Use this method to detect when a footer view is removed from a table view, as opposed to monitoring the view itself to see when it appears or disappears.

## See Also

### Tracking the removal of views

func tableView(UITableView, didEndDisplaying: UITableViewCell, forRowAt: IndexPath)

Tells the delegate that the specified cell was removed from the table.

func tableView(UITableView, didEndDisplayingHeaderView: UIView, forSection: Int)

Tells the delegate that the specified header view was removed from the table.

