

- UIKit
- UITableViewDelegate
-  tableView(\_:performPrimaryActionForRowAt:) 

Instance Method

# tableView(\_:performPrimaryActionForRowAt:)

Tells the delegate to perform the primary action for the row at the specified index path.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    performPrimaryActionForRowAt indexPath: IndexPath
)
```

## Parameters 

`tableView`  

The table view object on which to perform the primary action.

`indexPath`  

The index path of the row.

## Discussion

Primary actions allow you to distinguish between a distinct user action and a change in selection (like a focus change or other indirect selection change). A primary action occurs when a person selects a single row without extending an existing selection.

UIKit calls this method after tableView(_:willSelectRowAt:) and tableView(_:didSelectRowAt:), regardless of whether the row selection state changes. Use tableView(_:didSelectRowAt:) to update the state of the current view controller (like its buttons, title, and so on), and use tableView(_:performPrimaryActionForRowAt:) for actions like navigation or showing another split view column.

If tableView(_:willSelectRowAt:) returns an index path to allow selection for the row, only that row has selection when the system calls this method. If tableView(_:willSelectRowAt:) returns `nil`, the system preserves the existing row selection in the table view. You can use this behavior to perform primary actions on nonselectable, button-style rows without changing the selection.

## See Also

### Performing primary actions

func tableView(UITableView, canPerformPrimaryActionForRowAt: IndexPath) -> Bool

Asks the delegate whether to perform a primary action for the row at the specified index path.

