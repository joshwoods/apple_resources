

- UIKit
- UITableViewDelegate
-  tableView(\_:editingStyleForRowAt:) 

Instance Method

# tableView(\_:editingStyleForRowAt:)

Asks the delegate for the editing style of a row at a particular location in a table view.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    editingStyleForRowAt indexPath: IndexPath
) -> UITableViewCell.EditingStyle
```

## Parameters 

`tableView`  

The table view requesting this information.

`indexPath`  

An index path locating a row in `tableView`.

## Return Value

The editing style of the cell for the row identified by `indexPath`.

## Discussion

This method allows the delegate to customize the editing style of the cell located at`indexPath`. If the delegate does not implement this method and the `UITableViewCell` object is editable (that is, it has its isEditing property set to true), the cell has the UITableViewCell.EditingStyle.delete style set for it.

## See Also

### Editing table rows

func tableView(UITableView, willBeginEditingRowAt: IndexPath)

Tells the delegate that the table view is about to go into editing mode.

func tableView(UITableView, didEndEditingRowAt: IndexPath?)

Tells the delegate that the table view has left editing mode.

func tableView(UITableView, titleForDeleteConfirmationButtonForRowAt: IndexPath) -> String?

Changes the default title of the delete-confirmation button.

func tableView(UITableView, shouldIndentWhileEditingRowAt: IndexPath) -> Bool

Asks the delegate whether the background of the specified row should be indented while the table view is in editing mode.

