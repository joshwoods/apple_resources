

- AppKit
- NSOutlineViewDelegate
-  outlineView(\_:sizeToFitWidthOfColumn:) 

Instance Method

# outlineView(\_:sizeToFitWidthOfColumn:)

Invoked to allow the delegate to provide custom sizing behavior when a column’s resize divider is double clicked.

macOS 10.6+

``` source
@MainActor
optional func outlineView(
    _ outlineView: NSOutlineView,
    sizeToFitWidthOfColumn column: Int
) -> CGFloat
```

## Parameters 

`outlineView`  

The outline view that sent the message.

`column`  

The index of the column.

## Return Value

The width of the specified column.

## Discussion

By default, `NSOutlineView` iterates every row in the table, accesses a cell via preparedCell(atColumn:row:), and requests the cellSize to find the appropriate largest width to use.

For accurate results and performance, it is recommended that this method is implemented when using large tables. By default, large tables use a monte carlo simulation instead of iterating every row.

## See Also

### Customizing Column and Row Sizes

func outlineView(NSOutlineView, heightOfRowByItem: Any) -> CGFloat

Returns the height in points of the row containing `item`.

