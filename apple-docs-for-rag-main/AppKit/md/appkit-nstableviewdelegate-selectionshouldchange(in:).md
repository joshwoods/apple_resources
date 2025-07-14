

- AppKit
- NSTableViewDelegate
-  selectionShouldChange(in:) 

Instance Method

# selectionShouldChange(in:)

Asks the delegate if the user is allowed to change the selection.

macOS

``` source
@MainActor
optional func selectionShouldChange(in tableView: NSTableView) -> Bool
```

## Parameters 

`tableView`  

The table view that sent the message.

## Return Value

true to allow the table view to change its selection (typically a row being edited), false to deny selection change.

## Discussion

The user can select and edit different cells within the same row, but can’t select another row unless the delegate approves. The delegate can implement this method for complex validation of edited rows based on the values of any of their cells.

## See Also

### Selecting rows

func tableView(NSTableView, shouldSelectRow: Int) -> Bool

Asks the delegate if the table view should allow selection of the specified row.

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

