

- UIKit
- UITableViewDropDelegate
-  tableView(\_:dropSessionDidEnd:) 

Instance Method

# tableView(\_:dropSessionDidEnd:)

Notifies the delegate when the drag operation ends.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    dropSessionDidEnd session: any UIDropSession
)
```

## Parameters 

`tableView`  

The table view that is no longer the target of the drop.

`session`  

The drop session object containing information about the data being dragged.

## Discussion

The table view calls this method at the conclusion of a drag that was over the table view at one point. Use it to clean up any state information that you used to handle the drag. This method is called regardless of whether the data was actually dropped onto the table view.

## See Also

### Tracking the drag movements

func tableView(UITableView, dropSessionDidUpdate: any UIDropSession, withDestinationIndexPath: IndexPath?) -> UITableViewDropProposal

Proposes how to handle a drop at the specified location in the table view.

func tableView(UITableView, dropSessionDidEnter: any UIDropSession)

Notifies the delegate when dragged content enters the table view’s bounds rectangle.

func tableView(UITableView, dropSessionDidExit: any UIDropSession)

Notifies the delegate when dragged content exits the table view’s bounds rectangle.

