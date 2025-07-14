

- AppKit
- NSTableViewDelegate
-  tableView(\_:shouldSelectRow:) 

Instance Method

# tableView(\_:shouldSelectRow:)

Asks the delegate if the table view should allow selection of the specified row.

macOS

``` source
@MainActor
optional func tableView(
    _ tableView: NSTableView,
    shouldSelectRow row: Int
) -> Bool
```

## Parameters 

`tableView`  

The table view that sent the message.

`row`  

The row index.

## Return Value

true to permit selection of the row, false to deny selection.

## Discussion

The delegate can implement this method to disallow selection of particular rows.

For better performance and finer-grain control over the selection, use tableView(_:selectionIndexesForProposedSelection:).

## See Also

### Selecting rows

func selectionShouldChange(in: NSTableView) -> Bool

Asks the delegate if the user is allowed to change the selection.

func tableView(NSTableView, selectionIndexesForProposedSelection: IndexSet) -> IndexSet

Asks the delegate to accept or reject the proposed selection.

func tableView(NSTableView, shouldSelect: NSTableColumn?) -> Bool

Asks the delegate whether the specified table column can be selected.

func tableViewSelectionIsChanging(Notification)

Tells the delegate that the table view’s selection is in the process of changing.

func tableViewSelectionDidChange(Notification)

Tells the delegate that the table view’s selection has changed.

func tableView(NSTableView, shouldTypeSelectFor: NSEvent, withCurrentSearch: String?) -> Bool

Asks the delegate to allow or deny type select for the specified event and current search string.

func tableView(NSTableView, typeSelectStringFor: NSTableColumn?, row: Int) -> String?

Asks the delegate to provide an alternative text value used for type selection for the specified row and column.

func tableView(NSTableView, nextTypeSelectMatchFromRow: Int, toRow: Int, for: String) -> Int

Asks the delegate for the row within the specified search range that matches the specified string.

