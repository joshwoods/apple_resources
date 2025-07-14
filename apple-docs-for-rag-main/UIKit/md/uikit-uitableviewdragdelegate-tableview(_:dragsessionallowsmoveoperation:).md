

- UIKit
- UITableViewDragDelegate
-  tableView(\_:dragSessionAllowsMoveOperation:) 

Instance Method

# tableView(\_:dragSessionAllowsMoveOperation:)

Returns a Boolean value indicating whether your app supports a move operation for the dragged content.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    dragSessionAllowsMoveOperation session: any UIDragSession
) -> Bool
```

## Parameters 

`tableView`  

The table view from which the drag operation originated.

`session`  

The drag session object containing information about the drag operation.

## Return Value

true if your app allows content to be moved instead of copied, or false if moves are not supported.

## Discussion

Implement this method if you want to prevent the dragged content from being moved. If your delegate returns false and the drop operation type is UIDropOperation.move, the system cancels the drop.

If you don’t implement this method, the table view behaves as if the method returned true.

## See Also

### Tracking the drag session

func tableView(UITableView, dragSessionWillBegin: any UIDragSession)

Signals the start of a drag operation involving content from the specified table view.

func tableView(UITableView, dragSessionDidEnd: any UIDragSession)

Signals the end of a drag operation involving content from the specified table view.

func tableView(UITableView, dragSessionIsRestrictedToDraggingApplication: any UIDragSession) -> Bool

Returns a Boolean value indicating whether the dragged content must be dropped in the same app.

