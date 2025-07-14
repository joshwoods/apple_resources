

- AppKit
- NSTableColumn
-  width 

Instance Property

# width

The table column’s width, in points.

macOS

``` source
@MainActor
var width: CGFloat { get set }
```

## Discussion

The default value of this property is `100.0`.

If the value of this property exceeds the minimum or maximum width, it’s adjusted to the appropriate limiting value.

This property posts columnDidResizeNotification on behalf of the table column’s `NSTableView` and marks the table view as needing display.

## See Also

### Controlling Size

var minWidth: CGFloat

The table column’s minimum width, in points.

var maxWidth: CGFloat

The table column’s maximum width, in points.

var resizingMask: NSTableColumn.ResizingOptions

The table column’s resizing mask.

func sizeToFit()

Resizes the table column to fit the width of its header cell.

