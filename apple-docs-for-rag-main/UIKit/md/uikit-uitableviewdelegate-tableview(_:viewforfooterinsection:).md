

- UIKit
- UITableViewDelegate
-  tableView(\_:viewForFooterInSection:) 

Instance Method

# tableView(\_:viewForFooterInSection:)

Asks the delegate for a view to display in the footer of the specified section of the table view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    viewForFooterInSection section: Int
) -> UIView?
```

## Parameters 

`tableView`  

The table view asking for the view.

`section`  

The index number of the section containing the footer view.

## Return Value

A UILabel, UIImageView, or custom view to display at the bottom of the specified section.

## Mentioned in 

Adding headers and footers to table sections

## Discussion

If you implement this method but don’t implement tableView(_:heightForFooterInSection:), the table view calculates the height automatically, or uses the value of sectionFooterHeight if set.

## See Also

### Providing custom header and footer views

func tableView(UITableView, viewForHeaderInSection: Int) -> UIView?

Asks the delegate for a view to display in the header of the specified section of the table view.

func tableView(UITableView, willDisplayHeaderView: UIView, forSection: Int)

Tells the delegate that the table is about to display the header view for the specified section.

func tableView(UITableView, willDisplayFooterView: UIView, forSection: Int)

Tells the delegate that the table is about to display the footer view for the specified section.

