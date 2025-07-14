

- UIKit
- UITableViewCell
-  showingDeleteConfirmation 

Instance Property

# showingDeleteConfirmation

A Boolean value that indicates whether the cell is currently showing the delete-confirmation button.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var showingDeleteConfirmation: Bool { get }
```

## Discussion

When users tap the deletion control (the red circle to the left of the cell), the cell displays a “Delete” button on the right side of the cell; this string is localized.

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

var showsReorderControl: Bool

A Boolean value that determines whether the cell shows the reordering control.

