

- AppKit
- NSTableViewDelegate
-  tableView(\_:shouldShowCellExpansionFor:row:) 

Instance Method

# tableView(\_:shouldShowCellExpansionFor:row:)

Asks the delegate if an expansion tooltip should be displayed for a specific row and column.

macOS 10.5+

``` source
@MainActor
optional func tableView(
    _ tableView: NSTableView,
    shouldShowCellExpansionFor tableColumn: NSTableColumn?,
    row: Int
) -> Bool
```

## Parameters 

`tableView`  

The table view that sent the message.

`tableColumn`  

The table column.

`row`  

The row index.

## Return Value

true if an expansion tooltip should be displayed, false otherwise.

## Discussion

An expansion tooltip can be displayed when the pointer hovers over a cell that contains truncated text. When this method returns true, the cell’s full contents is shown in an expansion tooltip, which looks similar to a help tag.

Note

This method is only valid for NSCell-based table views.

## See Also

### Providing cells for rows and columns

func tableView(NSTableView, willDisplayCell: Any, for: NSTableColumn?, row: Int)

Tells the delegate that the table view will display the specified cell at the specified row and column.

func tableView(NSTableView, dataCellFor: NSTableColumn?, row: Int) -> NSCell?

Asks the delegate for a custom data cell for the specified row and column.

func tableView(NSTableView, toolTipFor: NSCell, rect: NSRectPointer, tableColumn: NSTableColumn?, row: Int, mouseLocation: NSPoint) -> String

Asks the delegate for a string to display in a tooltip for the specified cell in the column and row.

