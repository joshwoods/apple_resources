

- AppKit
- NSTableViewDelegate
-  tableView(\_:heightOfRow:) 

Instance Method

# tableView(\_:heightOfRow:)

Asks the delegate for the height of the specified row.

macOS 10.0+

``` source
@MainActor
optional func tableView(
    _ tableView: NSTableView,
    heightOfRow row: Int
) -> CGFloat
```

## Parameters 

`tableView`  

The table view that sent the message.

`row`  

The row index.

## Return Value

The height of the row. The height doesn’t include intercell spacing and must be greater than zero.

## Discussion

Implement this method if your table supports varying row heights.

Although table views may cache the returned values, you should ensure that this method is efficient. When you change a row’s height you must invalidate the existing row height by calling noteHeightOfRows(withIndexesChanged:). NSTableView automatically invalidates its entire row height cache in response to calls to reloadData() or noteNumberOfRowsChanged().

If you call view(atColumn:row:makeIfNecessary:) or rowView(atRow:makeIfNecessary:) within your implementation of this method, the table view throws an exception.

Important

To avoid the possibility of a hang due to unexpected recursion, don’t call geometry-calculating methods such as bounds, rect(ofColumn:), or any NSTableView method that calls tile() within your implementation of this method, such as intercellSpacing. To confirm your code isn’t inadvertently causing any calls to tile(), set a breakpoint on tile() in Xcode.

## See Also

### Setting row and column size

func tableView(NSTableView, sizeToFitWidthOfColumn: Int) -> CGFloat

Asks the delegate to provide custom sizing behavior when a column’s resize divider is double clicked.

