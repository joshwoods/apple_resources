

- UIKit
- UITableView
-  allowsSelection 

Instance Property

# allowsSelection

A Boolean value that determines whether users can select a row.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var allowsSelection: Bool { get set }
```

## Mentioned in 

Handling row selection in a table view

## Discussion

If the value of this property is true (the default), users can select rows. If you set it to false, they can’t select rows. Setting this property affects cell selection only when the table view isn’t in editing mode. If you want to restrict selection of cells in editing mode, use allowsSelectionDuringEditing.

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

var allowsMultipleSelection: Bool

A Boolean value that determines whether users can select more than one row outside of editing mode.

var allowsSelectionDuringEditing: Bool

A Boolean value that determines whether users can select cells while the table view is in editing mode.

var allowsMultipleSelectionDuringEditing: Bool

A Boolean value that controls whether users can select more than one cell simultaneously in editing mode.

var selectionFollowsFocus: Bool

A Boolean value that triggers an automatic selection when focus moves to a cell.

class let selectionDidChangeNotification: NSNotification.Name

A notification that posts when the selected row in the posting table view changes.

