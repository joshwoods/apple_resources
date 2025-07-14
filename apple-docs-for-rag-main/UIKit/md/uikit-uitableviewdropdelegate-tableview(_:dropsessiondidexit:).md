

- UIKit
- UITableViewDropDelegate
-  tableView(\_:dropSessionDidExit:) 

Instance Method

# tableView(\_:dropSessionDidExit:)

Notifies the delegate when dragged content exits the table view’s bounds rectangle.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    dropSessionDidExit session: any UIDropSession
)
```

## Parameters 

`tableView`  

The collection view that was tracking the dragged content.

`session`  

The drop session object containing information about the data being dragged.

## Discussion

The table view calls this method when dragged content exits its bounds rectangle. This method isn’t called again until the dragged content enters the table view’s bounds (triggering a call to the tableView(_:dropSessionDidEnter:) method) and exits again.

Use this method to clean up any state information that you configured in your tableView(_:dropSessionDidEnter:) method.

## See Also

### Tracking the drag movements

func tableView(UITableView, dropSessionDidUpdate: any UIDropSession, withDestinationIndexPath: IndexPath?) -> UITableViewDropProposal

Proposes how to handle a drop at the specified location in the table view.

func tableView(UITableView, dropSessionDidEnter: any UIDropSession)

Notifies the delegate when dragged content enters the table view’s bounds rectangle.

func tableView(UITableView, dropSessionDidEnd: any UIDropSession)

Notifies the delegate when the drag operation ends.

