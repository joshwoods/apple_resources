

- UIKit
- UITableViewDataSource
-  tableView(\_:titleForFooterInSection:) 

Instance Method

# tableView(\_:titleForFooterInSection:)

Asks the data source for the title of the footer of the specified section of the table view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    titleForFooterInSection section: Int
) -> String?
```

## Parameters 

`tableView`  

The table-view object asking for the title.

`section`  

An index number identifying a section of `tableView`.

## Return Value

A string to use as the title of the section footer. If you return `nil` , the section will have no title.

## Mentioned in 

Adding headers and footers to table sections

## Discussion

The table view uses a fixed font style for section footer titles. If you want a different font style, return a custom view (for example, a UILabel object) in the delegate method tableView(_:viewForFooterInSection:) instead.

If you don’t implement this method or the tableView(_:viewForFooterInSection:) method, the table doesn’t display footers for sections. If you implement both methods, the tableView(_:viewForFooterInSection:) method takes priority.

## See Also

### Providing cells, headers, and footers

func tableView(UITableView, cellForRowAt: IndexPath) -> UITableViewCell

Asks the data source for a cell to insert in a particular location of the table view.

**Required**

func tableView(UITableView, titleForHeaderInSection: Int) -> String?

Asks the data source for the title of the header of the specified section of the table view.

