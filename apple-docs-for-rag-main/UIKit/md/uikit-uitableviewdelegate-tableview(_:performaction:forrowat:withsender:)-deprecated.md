

- UIKit
- UITableViewDelegate
-  tableView(\_:performAction:forRowAt:withSender:) Deprecated

Instance Method

# tableView(\_:performAction:forRowAt:withSender:)

Tells the delegate to perform a copy or paste operation on the content of a given row.

iOS 5.0–13.0DeprecatediPadOS 5.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    performAction action: Selector,
    forRowAt indexPath: IndexPath,
    withSender sender: Any?
)
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

## Discussion

The table view invokes this method for a given `action` if the user taps Copy or Paste in the editing menu. The delegate can do whatever is appropriate for the action; for example, for a copy, it can extract the relevant cell content for the row at `indexPath` and write it to the general pasteboard or an application (private) pasteboard. See UIPasteboard for further information.

## See Also

### Responding to row actions

func tableView(UITableView, leadingSwipeActionsConfigurationForRowAt: IndexPath) -> UISwipeActionsConfiguration?

Returns the swipe actions to display on the leading edge of the row.

func tableView(UITableView, trailingSwipeActionsConfigurationForRowAt: IndexPath) -> UISwipeActionsConfiguration?

Returns the swipe actions to display on the trailing edge of the row.

func tableView(UITableView, shouldShowMenuForRowAt: IndexPath) -> Bool

Asks the delegate if the editing menu should be shown for a certain row.

Deprecated

func tableView(UITableView, canPerformAction: Selector, forRowAt: IndexPath, withSender: Any?) -> Bool

Asks the delegate if the editing menu should omit the Copy or Paste command for a given row.

Deprecated

func tableView(UITableView, editActionsForRowAt: IndexPath) -> [UITableViewRowAction]?

Asks the delegate for the actions to display in response to a swipe in the specified row.

Deprecated

