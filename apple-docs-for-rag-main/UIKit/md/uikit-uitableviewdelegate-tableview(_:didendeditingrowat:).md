

- UIKit
- UITableViewDelegate
-  tableView(\_:didEndEditingRowAt:) 

Instance Method

# tableView(\_:didEndEditingRowAt:)

Tells the delegate that the table view has left editing mode.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    didEndEditingRowAt indexPath: IndexPath?
)
```

## Parameters 

`tableView`  

The table view providing this information.

`indexPath`  

An index path locating the row in `tableView`.

## Discussion

This method is called when the table view exits editing mode after having been put into the mode by the user swiping across the row identified by `indexPath`. As a result, a Delete button appears in the row; however, in this “swipe to delete” mode the table view does not display any insertion, deletion, and reordering controls. When entering this “swipe to delete” editing mode, the table view sends a tableView(_:willBeginEditingRowAt:) message to the delegate to allow it to adjust its user interface.

## See Also

### Editing table rows

func tableView(UITableView, willBeginEditingRowAt: IndexPath)

Tells the delegate that the table view is about to go into editing mode.

func tableView(UITableView, editingStyleForRowAt: IndexPath) -> UITableViewCell.EditingStyle

Asks the delegate for the editing style of a row at a particular location in a table view.

func tableView(UITableView, titleForDeleteConfirmationButtonForRowAt: IndexPath) -> String?

Changes the default title of the delete-confirmation button.

func tableView(UITableView, shouldIndentWhileEditingRowAt: IndexPath) -> Bool

Asks the delegate whether the background of the specified row should be indented while the table view is in editing mode.

