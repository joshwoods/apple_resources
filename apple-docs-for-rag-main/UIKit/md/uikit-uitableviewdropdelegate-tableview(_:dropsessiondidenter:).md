

- UIKit
- UITableViewDropDelegate
-  tableView(\_:dropSessionDidEnter:) 

Instance Method

# tableView(\_:dropSessionDidEnter:)

Notifies the delegate when dragged content enters the table view’s bounds rectangle.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    dropSessionDidEnter session: any UIDropSession
)
```

## Parameters 

`tableView`  

The table view that’s now the potential target of the drop.

`session`  

The drop session object containing information about the data being dragged.

## Discussion

The table view calls this method when dragged content first enters its bounds rectangle. This method isn’t called again until the dragged content exits the table view’s bounds (triggering a call to the tableView(_:dropSessionDidExit:) method) and enters again.

Use this method to perform any one-time setup associated with tracking dragged content over the table view.

## See Also

### Tracking the drag movements

func tableView(UITableView, dropSessionDidUpdate: any UIDropSession, withDestinationIndexPath: IndexPath?) -> UITableViewDropProposal

Proposes how to handle a drop at the specified location in the table view.

func tableView(UITableView, dropSessionDidExit: any UIDropSession)

Notifies the delegate when dragged content exits the table view’s bounds rectangle.

func tableView(UITableView, dropSessionDidEnd: any UIDropSession)

Notifies the delegate when the drag operation ends.

