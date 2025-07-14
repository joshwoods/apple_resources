

- UIKit
- UITableViewDelegate
-  tableView(\_:shouldShowMenuForRowAt:) Deprecated

Instance Method

# tableView(\_:shouldShowMenuForRowAt:)

Asks the delegate if the editing menu should be shown for a certain row.

iOS 5.0–13.0DeprecatediPadOS 5.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    shouldShowMenuForRowAt indexPath: IndexPath
) -> Bool
```

## Parameters 

`tableView`  

The table view that is making this request.

`indexPath`  

The index path of the row.

## Return Value

true if the editing menu should be shown positioned near the row and pointing to it, otherwise false. The default value is false.

## Discussion

If the user tap-holds a certain row in the table view, this method (if implemented) is invoked first. Return false if the editing menu shouldn’t be shown—for example, the cell corresponding to the row contains content that shouldn’t be copied or pasted over.

## See Also

### Responding to row actions

func tableView(UITableView, leadingSwipeActionsConfigurationForRowAt: IndexPath) -> UISwipeActionsConfiguration?

Returns the swipe actions to display on the leading edge of the row.

func tableView(UITableView, trailingSwipeActionsConfigurationForRowAt: IndexPath) -> UISwipeActionsConfiguration?

Returns the swipe actions to display on the trailing edge of the row.

func tableView(UITableView, canPerformAction: Selector, forRowAt: IndexPath, withSender: Any?) -> Bool

Asks the delegate if the editing menu should omit the Copy or Paste command for a given row.

Deprecated

func tableView(UITableView, performAction: Selector, forRowAt: IndexPath, withSender: Any?)

Tells the delegate to perform a copy or paste operation on the content of a given row.

Deprecated

func tableView(UITableView, editActionsForRowAt: IndexPath) -> [UITableViewRowAction]?

Asks the delegate for the actions to display in response to a swipe in the specified row.

Deprecated

