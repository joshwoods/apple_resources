

- UIKit
- UITableViewDelegate
-  tableView(\_:willDisplayFooterView:forSection:) 

Instance Method

# tableView(\_:willDisplayFooterView:forSection:)

Tells the delegate that the table is about to display the footer view for the specified section.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    willDisplayFooterView view: UIView,
    forSection section: Int
)
```

## Parameters 

`tableView`  

The table view informing the delegate of this event.

`view`  

The footer view that is about to be displayed.

`section`  

The index number of the section containing the footer view.

## See Also

### Providing custom header and footer views

func tableView(UITableView, viewForHeaderInSection: Int) -> UIView?

Asks the delegate for a view to display in the header of the specified section of the table view.

func tableView(UITableView, viewForFooterInSection: Int) -> UIView?

Asks the delegate for a view to display in the footer of the specified section of the table view.

func tableView(UITableView, willDisplayHeaderView: UIView, forSection: Int)

Tells the delegate that the table is about to display the header view for the specified section.

