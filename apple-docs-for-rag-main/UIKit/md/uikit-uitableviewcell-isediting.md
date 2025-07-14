

- UIKit
- UITableViewCell
-  isEditing 

Instance Property

# isEditing

A Boolean value that indicates whether the cell is in an editable state.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isEditing: Bool { get set }
```

## Discussion

When a cell is in an editable state, it displays the editing controls specified for it: the green insertion control, the red deletion control, or (on the right side) the reordering control. Use editingStyle and showsReorderControl to specify these controls for the cell.

## See Also

### Editing the cell

func setEditing(Bool, animated: Bool)

Toggles the cell into and out of editing mode.

var editingStyle: UITableViewCell.EditingStyle

The editing style of the cell.

enum EditingStyle

The editing control used by a cell.

var showingDeleteConfirmation: Bool

A Boolean value that indicates whether the cell is currently showing the delete-confirmation button.

var showsReorderControl: Bool

A Boolean value that determines whether the cell shows the reordering control.

