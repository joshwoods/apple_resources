

- UIKit
- UITableViewDragDelegate
-  tableView(\_:dragSessionWillBegin:) 

Instance Method

# tableView(\_:dragSessionWillBegin:)

Signals the start of a drag operation involving content from the specified table view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    dragSessionWillBegin session: any UIDragSession
)
```

## Parameters 

`tableView`  

The table view from which the drag operation originated.

`session`  

The drag session object providing context for the drag operation.

## Discussion

This method is called after it has been determined that a drag will begin, after any lift animations have occurred, and before the position of the drag changes significantly. Use this method to perform any tasks related to the management of the drag session in your app.

Each call to this method is always balanced by a call to the tableView(_:dragSessionDidEnd:) method.

## See Also

### Tracking the drag session

func tableView(UITableView, dragSessionDidEnd: any UIDragSession)

Signals the end of a drag operation involving content from the specified table view.

func tableView(UITableView, dragSessionIsRestrictedToDraggingApplication: any UIDragSession) -> Bool

Returns a Boolean value indicating whether the dragged content must be dropped in the same app.

func tableView(UITableView, dragSessionAllowsMoveOperation: any UIDragSession) -> Bool

Returns a Boolean value indicating whether your app supports a move operation for the dragged content.

