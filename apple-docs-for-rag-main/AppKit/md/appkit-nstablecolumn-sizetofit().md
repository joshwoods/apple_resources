

- AppKit
- NSTableColumn
-  sizeToFit() 

Instance Method

# sizeToFit()

Resizes the table column to fit the width of its header cell.

macOS

``` source
@MainActor
func sizeToFit()
```

## Discussion

If the table column’s maximum width is less than the width of the header, the maximum is increased to the header’s width. Similarly, if the table column’s minimum width is greater than the width of the header, the minimum is reduced to the header’s width.

If this method causes the table column’s width to change, the column’s table view is marked as needing display.

## See Also

### Controlling Size

var width: CGFloat

The table column’s width, in points.

var minWidth: CGFloat

The table column’s minimum width, in points.

var maxWidth: CGFloat

The table column’s maximum width, in points.

var resizingMask: NSTableColumn.ResizingOptions

The table column’s resizing mask.

