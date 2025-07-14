

- UIKit
- UITableViewDelegate
-  tableView(\_:willSelectRowAt:) 

Instance Method

# tableView(\_:willSelectRowAt:)

Tells the delegate a row is about to be selected.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    willSelectRowAt indexPath: IndexPath
) -> IndexPath?
```

## Parameters 

`tableView`  

A table view informing the delegate about the impending selection.

`indexPath`  

An index path locating the row in `tableView`.

## Return Value

An index path that confirms or alters the selected row. Return an IndexPath (Swift) or NSIndexPath (Objective-C) other than `indexPath` if you want another cell to be selected. Return `nil` if you don’t want the row selected.

## Mentioned in 

Handling row selection in a table view

## Discussion

The system calls this method after a user has lifted their finger; the row is highlighted on the initial touch, but only selected when the touch withdraws. You can use UITableViewCell.SelectionStyle.none to disable the appearance of the cell highlight on the initial touch. The system doesn’t call this method if the rows in the table aren’t selectable. See Handling row selection in a table view for more information on controlling table row selection behavior.

## See Also

### Related Documentation

func tableView(UITableView, shouldIndentWhileEditingRowAt: IndexPath) -> Bool

Asks the delegate whether the background of the specified row should be indented while the table view is in editing mode.

### Responding to row selections

Handling row selection in a table view

Detect when a user taps a table view cell so your app can take the next indicated action.

Selecting multiple items with a two-finger pan gesture

Accelerate user selection of multiple items using the multiselect gesture on table and collection views.

func tableView(UITableView, didSelectRowAt: IndexPath)

Tells the delegate a row is selected.

func tableView(UITableView, willDeselectRowAt: IndexPath) -> IndexPath?

Tells the delegate that a specified row is about to be deselected.

func tableView(UITableView, didDeselectRowAt: IndexPath)

Tells the delegate that the specified row is now deselected.

func tableView(UITableView, shouldBeginMultipleSelectionInteractionAt: IndexPath) -> Bool

Asks the delegate whether the user can use a two-finger pan gesture to select multiple items in a table view.

func tableView(UITableView, didBeginMultipleSelectionInteractionAt: IndexPath)

Tells the delegate when the user starts using a two-finger pan gesture to select multiple rows in a table view.

func tableViewDidEndMultipleSelectionInteraction(UITableView)

Tells the delegate when the user stops using a two-finger pan gesture to select multiple rows in a table view.

