

- UIKit
- UITableViewCell
-  editingStyle 

Instance Property

# editingStyle

The editing style of the cell.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var editingStyle: UITableViewCell.EditingStyle { get }
```

## Discussion

One of the constants described in UITableViewCell.EditingStyle is used as the value of this property; it specifies whether the cell is in an editable state and, if it is, whether it shows an insertion or deletion control. The default value is UITableViewCell.EditingStyle.none (not editable). The delegate returns the value of this property for a particular cell in its implementation of the tableView(_:editingStyleForRowAt:) method.

## See Also

### Editing the cell

var isEditing: Bool

A Boolean value that indicates whether the cell is in an editable state.

func setEditing(Bool, animated: Bool)

Toggles the cell into and out of editing mode.

enum EditingStyle

The editing control used by a cell.

var showingDeleteConfirmation: Bool

A Boolean value that indicates whether the cell is currently showing the delete-confirmation button.

var showsReorderControl: Bool

A Boolean value that determines whether the cell shows the reordering control.

