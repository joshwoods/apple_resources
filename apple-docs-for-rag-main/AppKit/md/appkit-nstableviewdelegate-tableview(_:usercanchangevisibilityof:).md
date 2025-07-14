

- AppKit
- NSTableViewDelegate
-  tableView(\_:userCanChangeVisibilityOf:) 

Instance Method

# tableView(\_:userCanChangeVisibilityOf:)

Asks the delegate to verify that the user can change the given column’s visibility.

macOS 14.0+

``` source
optional func tableView(
    _ tableView: NSTableView,
    userCanChangeVisibilityOf column: NSTableColumn
) -> Bool
```

## Parameters 

`tableView`  

The table view object requesting this information.

`column`  

The table column affected by the visibility change.

## Return Value

true if the user can change the visibility of the column; otherwise, false.

## Discussion

Implement this method to enable the table view to provide a menu that allows users to show or hide table columns.

To change a column’s visibility, ensure the column has a title. Further, setting the menu property on the table view headerView or, subclassing NSTableHeaderView and overriding the menu property also prevents the column visibility from changing.

## See Also

### Showing and hiding columns

func tableView(NSTableView, userDidChangeVisibilityOf: [NSTableColumn])

Tells the delegate that the user changed the visibility of one or more table columns.

