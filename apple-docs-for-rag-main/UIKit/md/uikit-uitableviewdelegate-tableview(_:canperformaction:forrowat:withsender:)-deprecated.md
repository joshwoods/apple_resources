

- UIKit
- UITableViewDelegate
-  tableView(\_:canPerformAction:forRowAt:withSender:) Deprecated

Instance Method

# tableView(\_:canPerformAction:forRowAt:withSender:)

Asks the delegate if the editing menu should omit the Copy or Paste command for a given row.

iOS 5.0–13.0DeprecatediPadOS 5.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    canPerformAction action: Selector,
    forRowAt indexPath: IndexPath,
    withSender sender: Any?
) -> Bool
```

## Parameters 

`tableView`  

The table view that is making this request.

`action`  

A selector type identifying the copy(_:) or paste(_:) method of the UIResponderStandardEditActions informal protocol.

`indexPath`  

The index path of the row.

`sender`  

The object that initially sent the `copy:` or `paste:` message.

## Return Value

true if the command corresponding to `action` should appear in the editing menu, otherwise false. The default value is false.

## Discussion

This method is invoked after tableView(_:shouldShowMenuForRowAt:). It gives the developer the opportunity to exclude one of the commands—Copy or Paste—from the editing menu. For example, the user might have copied some cell content from one row but wants to paste into another row that doesn’t take the copied content. In a case like this, return false from this method.

## See Also

### Responding to row actions

func tableView(UITableView, leadingSwipeActionsConfigurationForRowAt: IndexPath) -> UISwipeActionsConfiguration?

Returns the swipe actions to display on the leading edge of the row.

func tableView(UITableView, trailingSwipeActionsConfigurationForRowAt: IndexPath) -> UISwipeActionsConfiguration?

Returns the swipe actions to display on the trailing edge of the row.

func tableView(UITableView, shouldShowMenuForRowAt: IndexPath) -> Bool

Asks the delegate if the editing menu should be shown for a certain row.

Deprecated

func tableView(UITableView, performAction: Selector, forRowAt: IndexPath, withSender: Any?)

Tells the delegate to perform a copy or paste operation on the content of a given row.

Deprecated

func tableView(UITableView, editActionsForRowAt: IndexPath) -> [UITableViewRowAction]?

Asks the delegate for the actions to display in response to a swipe in the specified row.

Deprecated

