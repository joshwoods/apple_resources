

- UIKit
- UITableView
-  allowsMultipleSelection 

Instance Property

# allowsMultipleSelection

A Boolean value that determines whether users can select more than one row outside of editing mode.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var allowsMultipleSelection: Bool { get set }
```

## Mentioned in 

Handling row selection in a table view

## Discussion

This property controls whether a user can select multiple rows simultaneously outside of editing mode. Selected rows acquire a selected appearance.

In iOS, when the value of this property is true, the user can select additional rows by tapping on them. The user must tap a currently selected row to deselect it.

In macOS, when the value of this property is true, the user can select additional rows by holding the Command or Shift key while clicking on the additional rows they want to select. If the user isn’t holding a modifier key, clicking on another row clears the current selection and selects only the clicked row. This behavior resembles the selection behavior of NSTableView.

If you access indexPathsForSelectedRows, you can get the index paths that identify the selected rows.

The default value of this property is false.

## See Also

### Selecting rows

var indexPathForSelectedRow: IndexPath?

An index path that identifies the row and section of the selected row.

var indexPathsForSelectedRows: [IndexPath]?

The index paths that represent the selected rows.

func selectRow(at: IndexPath?, animated: Bool, scrollPosition: UITableView.ScrollPosition)

Selects a row in the table view that an index path identifies, optionally scrolling the row to a location in the table view.

func deselectRow(at: IndexPath, animated: Bool)

Deselects a row that an index path identifies, with an option to animate the deselection.

var allowsSelection: Bool

A Boolean value that determines whether users can select a row.

var allowsSelectionDuringEditing: Bool

A Boolean value that determines whether users can select cells while the table view is in editing mode.

var allowsMultipleSelectionDuringEditing: Bool

A Boolean value that controls whether users can select more than one cell simultaneously in editing mode.

var selectionFollowsFocus: Bool

A Boolean value that triggers an automatic selection when focus moves to a cell.

class let selectionDidChangeNotification: NSNotification.Name

A notification that posts when the selected row in the posting table view changes.

