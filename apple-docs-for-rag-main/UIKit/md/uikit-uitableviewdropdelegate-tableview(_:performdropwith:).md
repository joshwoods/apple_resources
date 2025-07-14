

- UIKit
- UITableViewDropDelegate
-  tableView(\_:performDropWith:) 

Instance Method

# tableView(\_:performDropWith:)

Incorporates the dropped data into your data structures and updates the table.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func tableView(
    _ tableView: UITableView,
    performDropWith coordinator: any UITableViewDropCoordinator
)
```

**Required**

## Parameters 

`tableView`  

The table view that received the drop.

`coordinator`  

The coordinator object to use when handling the drop. Use this object to coordinate your custom behavior with the default behavior of the table view.

## Mentioned in 

Supporting drag and drop in table views

## Discussion

Use this method to integrate the dropped content into your table view. In your implementation, iterate over the items property of the `coordinator` object to retrieve the UIDragItem objects associated with the drag operation. Use the data in those objects to update your table view’s data source and the table view itself.

How you update the table view depends on the source of the dragged items and whether you need to load the data asynchronously.

- **Insert placeholder rows for any data that you must load asynchronously.** Use the `drop(_:toPlaceholderInsertedAt:withReuseIdentifier:rowHeight:cellUpdateHandler:)` method to insert a placeholder cell into the table while you wait for the data to load.

- **Use the existing table view methods to rearrange rows within the table.** When the drag source contains rows from the same table, use the moveRow(at:to:) method to rearrange the rows.

- **Insert local data directly into the table.** When the drag item’s localObject property contains a value, use that value to update the table view directly. Specifically, update your data source object and insert any needed rows into the table.

When updating your table directly, use the coordinator object to animate the dropping of the items. For example, you might use the drop(_:toRowAt:) method to animate the insertion of the dropped item at the specified location. The insertion of placeholders automatically creates appropriate animations. For more information about the types of animations that you can perform, see UITableViewDropCoordinator.

