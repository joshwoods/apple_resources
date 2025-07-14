

- UIKit
- UITableViewCell
-  showsReorderControl 

Instance Property

# showsReorderControl

A Boolean value that determines whether the cell shows the reordering control.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var showsReorderControl: Bool { get set }
```

## Discussion

The reordering control is gray, multiple horizontal bar control on the right side of the cell. Users can drag this control to reorder the cell within the table. The default value is false. If the value is true , the reordering control temporarily replaces any accessory view.

For the reordering control to appear, you must not only set this property but implement the UITableViewDataSource method tableView(_:moveRowAt:to:). In addition, if the data source implements tableView(_:canMoveRowAt:) to return false, the reordering control doesn’t appear in that designated row.

## See Also

### Editing the cell

var isEditing: Bool

A Boolean value that indicates whether the cell is in an editable state.

func setEditing(Bool, animated: Bool)

Toggles the cell into and out of editing mode.

var editingStyle: UITableViewCell.EditingStyle

The editing style of the cell.

enum EditingStyle

The editing control used by a cell.

var showingDeleteConfirmation: Bool

A Boolean value that indicates whether the cell is currently showing the delete-confirmation button.

