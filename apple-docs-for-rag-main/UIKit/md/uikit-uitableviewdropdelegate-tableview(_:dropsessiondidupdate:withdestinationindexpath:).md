

- UIKit
- UITableViewDropDelegate
-  tableView(\_:dropSessionDidUpdate:withDestinationIndexPath:) 

Instance Method

# tableView(\_:dropSessionDidUpdate:withDestinationIndexPath:)

Proposes how to handle a drop at the specified location in the table view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    dropSessionDidUpdate session: any UIDropSession,
    withDestinationIndexPath destinationIndexPath: IndexPath?
) -> UITableViewDropProposal
```

## Parameters 

`tableView`  

The table view currently being targeted to receive the drop.

`session`  

The drop session object containing information about the data being dragged.

`destinationIndexPath`  

The index path of the row currently being targeted by the drop. Use this value to determine an appropriate course of action for the drop.

## Return Value

The UITableViewDropProposal object indicating how to incorporate the dropped data.

## Mentioned in 

Supporting drag and drop in table views

## Discussion

While the user is dragging content, the table view calls this method repeatedly to determine how you would handle the drop if it occurred at the specified location. The table view provides visual feedback to the user based on your proposal.

In your implementation of this method, create a UITableViewDropProposal object and use it to convey your intentions. Because this method is called repeatedly while the user drags over the table view, your implementation should return as quickly as possible.

## See Also

### Tracking the drag movements

func tableView(UITableView, dropSessionDidEnter: any UIDropSession)

Notifies the delegate when dragged content enters the table view’s bounds rectangle.

func tableView(UITableView, dropSessionDidExit: any UIDropSession)

Notifies the delegate when dragged content exits the table view’s bounds rectangle.

func tableView(UITableView, dropSessionDidEnd: any UIDropSession)

Notifies the delegate when the drag operation ends.

