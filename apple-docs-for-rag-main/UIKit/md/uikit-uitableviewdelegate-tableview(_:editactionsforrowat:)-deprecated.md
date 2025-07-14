

- UIKit
- UITableViewDelegate
-  tableView(\_:editActionsForRowAt:) Deprecated

Instance Method

# tableView(\_:editActionsForRowAt:)

Asks the delegate for the actions to display in response to a swipe in the specified row.

iOS 8.0–13.0DeprecatediPadOS 8.0–13.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    editActionsForRowAt indexPath: IndexPath
) -> [UITableViewRowAction]?
```

## Parameters 

`tableView`  

The table view requesting this information.

`indexPath`  

The index path of the row.

## Return Value

An array of UITableViewRowAction objects representing the actions for the row. Each action you provide is used to create a button that the user can tap.

## Discussion

Use this method when you want to provide custom actions for one of your table rows. When the user swipes horizontally in a row, the table view moves the row content aside to reveal your actions. Tapping one of the action buttons executes the handler block stored with the action object.

If you do not implement this method, the table view displays the standard accessory buttons when the user swipes the row.

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

func tableView(UITableView, performAction: Selector, forRowAt: IndexPath, withSender: Any?)

Tells the delegate to perform a copy or paste operation on the content of a given row.

Deprecated

