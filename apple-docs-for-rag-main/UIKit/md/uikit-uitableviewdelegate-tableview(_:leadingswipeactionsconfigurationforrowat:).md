

- UIKit
- UITableViewDelegate
-  tableView(\_:leadingSwipeActionsConfigurationForRowAt:) 

Instance Method

# tableView(\_:leadingSwipeActionsConfigurationForRowAt:)

Returns the swipe actions to display on the leading edge of the row.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    leadingSwipeActionsConfigurationForRowAt indexPath: IndexPath
) -> UISwipeActionsConfiguration?
```

## Parameters 

`tableView`  

The table view containing the row.

`indexPath`  

The index path of the row.

## Return Value

The swipe actions to display next to the leading edge of the row. Return `nil` if you want the table to display the default set of actions.

## Discussion

Use this method to return a set of actions to display when the user swipes the row. The actions you return are displayed on the leading edge of the row. For example, in a left-to-right language environment, they are displayed on the left side of the row when the user swipes from left to right.

## See Also

### Responding to row actions

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

func tableView(UITableView, editActionsForRowAt: IndexPath) -> [UITableViewRowAction]?

Asks the delegate for the actions to display in response to a swipe in the specified row.

Deprecated

