

- UIKit
- UITableViewDataSource
-  tableView(\_:canMoveRowAt:) 

Instance Method

# tableView(\_:canMoveRowAt:)

Asks the data source whether a given row can move to another location in the table view.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    canMoveRowAt indexPath: IndexPath
) -> Bool
```

## Parameters 

`tableView`  

The table-view object requesting this information.

`indexPath`  

An index path locating a row in `tableView`.

## Return Value

true if the row can be moved; otherwise, false.

## Discussion

This method allows the data source to specify that the reordering control for the specified row not be shown. By default, the reordering control is shown if the data source implements the tableView(_:moveRowAt:to:) method.

## See Also

### Reordering table rows

func tableView(UITableView, moveRowAt: IndexPath, to: IndexPath)

Tells the data source to move a row at a specific location in the table view to another location.

