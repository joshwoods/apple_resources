

- AppKit
- NSTableViewDelegate
-  tableView(\_:sizeToFitWidthOfColumn:) 

Instance Method

# tableView(\_:sizeToFitWidthOfColumn:)

Asks the delegate to provide custom sizing behavior when a column’s resize divider is double clicked.

macOS 10.6+

``` source
@MainActor
optional func tableView(
    _ tableView: NSTableView,
    sizeToFitWidthOfColumn column: Int
) -> CGFloat
```

## Parameters 

`tableView`  

The table view that sent the message.

`column`  

The index of the column.

## Return Value

The width of the specified column.

## Discussion

By default, NSTableView iterates every row in the table, accesses a cell via preparedCell(atColumn:row:), and requests the cellSize to find the appropriate largest width to use.

For accurate results and performance, it’s recommended that this method is implemented when using large tables. By default, large tables use a Monte Carlo simulation instead of iterating every row.

## See Also

### Setting row and column size

func tableView(NSTableView, heightOfRow: Int) -> CGFloat

Asks the delegate for the height of the specified row.

