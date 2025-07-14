

- UIKit
- UITableViewCell
-  setEditing(\_:animated:) 

Instance Method

# setEditing(\_:animated:)

Toggles the cell into and out of editing mode.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setEditing(
    _ editing: Bool,
    animated: Bool
)
```

## Parameters 

`editing`  

true to enter editing mode, false to leave it. The default value is false.

`animated`  

true to animate the appearance or disappearance of the insertion/deletion control and the reordering control, false to make the transition immediate.

## Discussion

When you call this method with the value of `editing` set to true, and the `UITableViewCell` object is configured to have controls, the cell shows an insertion (green plus) or deletion control (red minus) on the left side of each cell and a reordering control on the right side. This method is called on each visible cell when the setEditing(_:animated:) method of `UITableView` is invoked. Calling this method with `editing` set to false removes the controls from the cell.

## See Also

### Editing the cell

var isEditing: Bool

A Boolean value that indicates whether the cell is in an editable state.

var editingStyle: UITableViewCell.EditingStyle

The editing style of the cell.

enum EditingStyle

The editing control used by a cell.

var showingDeleteConfirmation: Bool

A Boolean value that indicates whether the cell is currently showing the delete-confirmation button.

var showsReorderControl: Bool

A Boolean value that determines whether the cell shows the reordering control.

