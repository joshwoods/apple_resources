

- UIKit
- UITableView
-  indexPathsForSelectedRows 

Instance Property

# indexPathsForSelectedRows

The index paths that represent the selected rows.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var indexPathsForSelectedRows: [IndexPath]? { get }
```

## Discussion

The value of this property is an array of index-path objects each identifying a row through its section and row index. The value of this property is `nil` if there are no selected rows.

## See Also

### Selecting rows

var indexPathForSelectedRow: IndexPath?

An index path that identifies the row and section of the selected row.

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

class let selectionDidChangeNotification: NSNotification.Name

A notification that posts when the selected row in the posting table view changes.

