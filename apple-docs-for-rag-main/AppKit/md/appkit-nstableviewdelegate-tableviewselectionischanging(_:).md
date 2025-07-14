

- AppKit
- NSTableViewDelegate
-  tableViewSelectionIsChanging(\_:) 

Instance Method

# tableViewSelectionIsChanging(\_:)

Tells the delegate that the table view’s selection is in the process of changing.

macOS 10.10+

``` source
@MainActor
optional func tableViewSelectionIsChanging(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named selectionIsChangingNotification.

## Discussion

This method is called only when mouse events—and not keyboard events—are changing the selection. For example, this method is called when the user drags the mouse across multiple table rows.

## See Also

### Selecting rows

func selectionShouldChange(in: NSTableView) -> Bool

Asks the delegate if the user is allowed to change the selection.

func tableView(NSTableView, shouldSelectRow: Int) -> Bool

Asks the delegate if the table view should allow selection of the specified row.

func tableView(NSTableView, selectionIndexesForProposedSelection: IndexSet) -> IndexSet

Asks the delegate to accept or reject the proposed selection.

func tableView(NSTableView, shouldSelect: NSTableColumn?) -> Bool

Asks the delegate whether the specified table column can be selected.

func tableViewSelectionDidChange(Notification)

Tells the delegate that the table view’s selection has changed.

func tableView(NSTableView, shouldTypeSelectFor: NSEvent, withCurrentSearch: String?) -> Bool

Asks the delegate to allow or deny type select for the specified event and current search string.

func tableView(NSTableView, typeSelectStringFor: NSTableColumn?, row: Int) -> String?

Asks the delegate to provide an alternative text value used for type selection for the specified row and column.

func tableView(NSTableView, nextTypeSelectMatchFromRow: Int, toRow: Int, for: String) -> Int

Asks the delegate for the row within the specified search range that matches the specified string.

