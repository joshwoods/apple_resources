

- UIKit
- UITableViewDelegate
-  tableView(\_:shouldIndentWhileEditingRowAt:) 

Instance Method

# tableView(\_:shouldIndentWhileEditingRowAt:)

Asks the delegate whether the background of the specified row should be indented while the table view is in editing mode.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    shouldIndentWhileEditingRowAt indexPath: IndexPath
) -> Bool
```

## Parameters 

`tableView`  

The table view requesting this information.

`indexPath`  

An index path locating the row in its section.

## Return Value

true if the background of the row should be indented, otherwise false.

## Discussion

If the delegate does not implement this method, the default is true. This method is unrelated to tableView(_:indentationLevelForRowAt:).

## See Also

### Editing table rows

func tableView(UITableView, willBeginEditingRowAt: IndexPath)

Tells the delegate that the table view is about to go into editing mode.

func tableView(UITableView, didEndEditingRowAt: IndexPath?)

Tells the delegate that the table view has left editing mode.

func tableView(UITableView, editingStyleForRowAt: IndexPath) -> UITableViewCell.EditingStyle

Asks the delegate for the editing style of a row at a particular location in a table view.

func tableView(UITableView, titleForDeleteConfirmationButtonForRowAt: IndexPath) -> String?

Changes the default title of the delete-confirmation button.

