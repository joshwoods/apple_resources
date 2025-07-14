

- AppKit
- NSTableViewDelegate
-  tableView(\_:shouldTypeSelectFor:withCurrentSearch:) 

Instance Method

# tableView(\_:shouldTypeSelectFor:withCurrentSearch:)

Asks the delegate to allow or deny type select for the specified event and current search string.

macOS 10.5+

``` source
@MainActor
optional func tableView(
    _ tableView: NSTableView,
    shouldTypeSelectFor event: NSEvent,
    withCurrentSearch searchString: String?
) -> Bool
```

## Parameters 

`tableView`  

The table view that sent the message.

`event`  

The event.

`searchString`  

The search string or `nil` if no type select has began.

## Return Value

true to allow type select for event, false otherwise.

## Discussion

Typically, this is called from the NSTableView `keyDown:` implementation and the event will be a key event.

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

func tableViewSelectionIsChanging(Notification)

Tells the delegate that the table view’s selection is in the process of changing.

func tableViewSelectionDidChange(Notification)

Tells the delegate that the table view’s selection has changed.

func tableView(NSTableView, typeSelectStringFor: NSTableColumn?, row: Int) -> String?

Asks the delegate to provide an alternative text value used for type selection for the specified row and column.

func tableView(NSTableView, nextTypeSelectMatchFromRow: Int, toRow: Int, for: String) -> Int

Asks the delegate for the row within the specified search range that matches the specified string.

