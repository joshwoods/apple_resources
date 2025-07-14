

- UIKit
- UITableView
-  selectionDidChangeNotification 

Type Property

# selectionDidChangeNotification

A notification that posts when the selected row in the posting table view changes.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
nonisolated
class let selectionDidChangeNotification: NSNotification.Name
```

## Mentioned in 

Handling row selection in a table view

## Discussion

There’s no `userInfo` dictionary associated with this notification.

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

var allowsMultipleSelection: Bool

A Boolean value that determines whether users can select more than one row outside of editing mode.

var allowsSelectionDuringEditing: Bool

A Boolean value that determines whether users can select cells while the table view is in editing mode.

var allowsMultipleSelectionDuringEditing: Bool

A Boolean value that controls whether users can select more than one cell simultaneously in editing mode.

var selectionFollowsFocus: Bool

A Boolean value that triggers an automatic selection when focus moves to a cell.

