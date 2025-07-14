

- UIKit
- UITableViewDragDelegate
-  tableView(\_:dragSessionDidEnd:) 

Instance Method

# tableView(\_:dragSessionDidEnd:)

Signals the end of a drag operation involving content from the specified table view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    dragSessionDidEnd session: any UIDragSession
)
```

## Parameters 

`tableView`  

The table view from which the drag operation originated.

`session`  

The drag session object providing context for the drag operation.

## Discussion

This method is called after the drag session ended, usually because the content was dropped but possibly because the drag was terminated. Use this method to close out any tasks related to the management of the drag session in your app.

Each call to this method is always preceded by a call to the tableView(_:dragSessionWillBegin:) method.

## See Also

### Tracking the drag session

func tableView(UITableView, dragSessionWillBegin: any UIDragSession)

Signals the start of a drag operation involving content from the specified table view.

func tableView(UITableView, dragSessionIsRestrictedToDraggingApplication: any UIDragSession) -> Bool

Returns a Boolean value indicating whether the dragged content must be dropped in the same app.

func tableView(UITableView, dragSessionAllowsMoveOperation: any UIDragSession) -> Bool

Returns a Boolean value indicating whether your app supports a move operation for the dragged content.

