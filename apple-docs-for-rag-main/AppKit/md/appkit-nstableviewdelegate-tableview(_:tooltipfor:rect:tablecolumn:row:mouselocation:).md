

- AppKit
- NSTableViewDelegate
-  tableView(\_:toolTipFor:rect:tableColumn:row:mouseLocation:) 

Instance Method

# tableView(\_:toolTipFor:rect:tableColumn:row:mouseLocation:)

Asks the delegate for a string to display in a tooltip for the specified cell in the column and row.

macOS

``` source
@MainActor
optional func tableView(
    _ tableView: NSTableView,
    toolTipFor cell: NSCell,
    rect: NSRectPointer,
    tableColumn: NSTableColumn?,
    row: Int,
    mouseLocation: NSPoint
) -> String
```

## Parameters 

`tableView`  

The table view that sent the message.

`cell`  

The cell.

`rect`  

The proposed active area of the tooltip. You can modify `rect` to provide an alternative active area.

`tableColumn`  

The table column.

`row`  

The row index.

`mouseLocation`  

The mouse location.

## Return Value

A string that should be displayed in the tooltip. Return `nil` or the empty string if no tooltip is desired.

## Discussion

By default, `rect` is computed as

`[cell drawingRectForBounds:cellFrame]`. Note that tooltips are also known as help tags.

## See Also

### Providing cells for rows and columns

func tableView(NSTableView, willDisplayCell: Any, for: NSTableColumn?, row: Int)

Tells the delegate that the table view will display the specified cell at the specified row and column.

func tableView(NSTableView, dataCellFor: NSTableColumn?, row: Int) -> NSCell?

Asks the delegate for a custom data cell for the specified row and column.

func tableView(NSTableView, shouldShowCellExpansionFor: NSTableColumn?, row: Int) -> Bool

Asks the delegate if an expansion tooltip should be displayed for a specific row and column.

