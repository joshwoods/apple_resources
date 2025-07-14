

- AppKit
- NSTableColumn
-  resizingMask 

Instance Property

# resizingMask

The table column’s resizing mask.

macOS

``` source
@MainActor
var resizingMask: NSTableColumn.ResizingOptions { get set }
```

## Discussion

The value of this property specifies the resizability of the table column. See Resizing Modes for possible values. Values can be combined using the C bitwise OR operator.

When the value of this property is `0`, the column is not resizable. The default value of this property is userResizingMask \| autoresizingMask.

## See Also

### Controlling Size

var width: CGFloat

The table column’s width, in points.

var minWidth: CGFloat

The table column’s minimum width, in points.

var maxWidth: CGFloat

The table column’s maximum width, in points.

func sizeToFit()

Resizes the table column to fit the width of its header cell.

