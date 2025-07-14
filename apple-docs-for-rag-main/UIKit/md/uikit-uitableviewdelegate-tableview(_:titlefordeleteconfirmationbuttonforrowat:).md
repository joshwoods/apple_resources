

- UIKit
- UITableViewDelegate
-  tableView(\_:titleForDeleteConfirmationButtonForRowAt:) 

Instance Method

# tableView(\_:titleForDeleteConfirmationButtonForRowAt:)

Changes the default title of the delete-confirmation button.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    titleForDeleteConfirmationButtonForRowAt indexPath: IndexPath
) -> String?
```

## Parameters 

`tableView`  

The table view requesting this information.

`indexPath`  

An index path locating the row in its section.

## Return Value

A localized string to used as the title of the delete-confirmation button.

## Discussion

By default, the delete-confirmation button, which appears on the right side of the cell, has the title of “Delete”. The table view displays this button when the user attempts to delete a row, either by swiping the row or tapping the red minus icon in editing mode. You can implement this method to return an alternative title, which should be localized.

## See Also

### Editing table rows

func tableView(UITableView, willBeginEditingRowAt: IndexPath)

Tells the delegate that the table view is about to go into editing mode.

func tableView(UITableView, didEndEditingRowAt: IndexPath?)

Tells the delegate that the table view has left editing mode.

func tableView(UITableView, editingStyleForRowAt: IndexPath) -> UITableViewCell.EditingStyle

Asks the delegate for the editing style of a row at a particular location in a table view.

func tableView(UITableView, shouldIndentWhileEditingRowAt: IndexPath) -> Bool

Asks the delegate whether the background of the specified row should be indented while the table view is in editing mode.

