

- AppKit
- NSTableViewDelegate
-  tableView(\_:shouldSelect:) 

Instance Method

# tableView(\_:shouldSelect:)

Asks the delegate whether the specified table column can be selected.

macOS

``` source
@MainActor
optional func tableView(
    _ tableView: NSTableView,
    shouldSelect tableColumn: NSTableColumn?
) -> Bool
```

## Parameters 

`tableView`  

The table view that sent the message.

`tableColumn`  

The table column.

## Return Value

true to permit selection, otherwise false.

## Discussion

The delegate can implement this method to disallow selection of particular columns.

## See Also

### Selecting rows

func selectionShouldChange(in: NSTableView) -> Bool

Asks the delegate if the user is allowed to change the selection.

func tableView(NSTableView, shouldSelectRow: Int) -> Bool

Asks the delegate if the table view should allow selection of the specified row.

func tableView(NSTableView, selectionIndexesForProposedSelection: IndexSet) -> IndexSet

Asks the delegate to accept or reject the proposed selection.

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

