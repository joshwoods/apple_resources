

- UIKit
- UITableViewDataSource
-  tableView(\_:moveRowAt:to:) 

Instance Method

# tableView(\_:moveRowAt:to:)

Tells the data source to move a row at a specific location in the table view to another location.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    moveRowAt sourceIndexPath: IndexPath,
    to destinationIndexPath: IndexPath
)
```

## Parameters 

`tableView`  

The table-view object requesting this action.

`sourceIndexPath`  

An index path locating the row to be moved in `tableView`.

`destinationIndexPath`  

An index path locating the row in `tableView` that’s the destination of the move.

## Discussion

The UITableView object sends this message to the data source when the user presses the reorder control in the row at `sourceIndexPath`.

## See Also

### Related Documentation

func tableView(UITableView, commit: UITableViewCell.EditingStyle, forRowAt: IndexPath)

Asks the data source to commit the insertion or deletion of a specified row.

### Reordering table rows

func tableView(UITableView, canMoveRowAt: IndexPath) -> Bool

Asks the data source whether a given row can move to another location in the table view.

