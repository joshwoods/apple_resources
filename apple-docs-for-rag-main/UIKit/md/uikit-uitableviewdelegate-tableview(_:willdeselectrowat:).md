

- UIKit
- UITableViewDelegate
-  tableView(\_:willDeselectRowAt:) 

Instance Method

# tableView(\_:willDeselectRowAt:)

Tells the delegate that a specified row is about to be deselected.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    willDeselectRowAt indexPath: IndexPath
) -> IndexPath?
```

## Parameters 

`tableView`  

A table view informing the delegate about the impending deselection.

`indexPath`  

An index path locating the row in `tableView` to be deselected.

## Return Value

An index path that confirms or alters the deselected row. Return an `NSIndexPath` object other than `indexPath` if you want another cell to be deselected. Return `nil` if you don’t want the row deselected.

## Discussion

This method is only called if there is an existing selection when the user tries to select a different row. The delegate is sent this method for the previously selected row. You can use UITableViewCell.SelectionStyle.none to disable the appearance of the cell highlight on touch-down.

## See Also

### Responding to row selections

Handling row selection in a table view

Detect when a user taps a table view cell so your app can take the next indicated action.

Selecting multiple items with a two-finger pan gesture

Accelerate user selection of multiple items using the multiselect gesture on table and collection views.

func tableView(UITableView, willSelectRowAt: IndexPath) -> IndexPath?

Tells the delegate a row is about to be selected.

func tableView(UITableView, didSelectRowAt: IndexPath)

Tells the delegate a row is selected.

func tableView(UITableView, didDeselectRowAt: IndexPath)

Tells the delegate that the specified row is now deselected.

func tableView(UITableView, shouldBeginMultipleSelectionInteractionAt: IndexPath) -> Bool

Asks the delegate whether the user can use a two-finger pan gesture to select multiple items in a table view.

func tableView(UITableView, didBeginMultipleSelectionInteractionAt: IndexPath)

Tells the delegate when the user starts using a two-finger pan gesture to select multiple rows in a table view.

func tableViewDidEndMultipleSelectionInteraction(UITableView)

Tells the delegate when the user stops using a two-finger pan gesture to select multiple rows in a table view.

