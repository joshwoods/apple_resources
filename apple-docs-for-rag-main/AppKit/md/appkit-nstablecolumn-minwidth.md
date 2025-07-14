

- AppKit
- NSTableColumn
-  minWidth 

Instance Property

# minWidth

The table column’s minimum width, in points.

macOS

``` source
@MainActor
var minWidth: CGFloat { get set }
```

## Discussion

The default value of this property is `10.0`.

The table column width can’t be less than the value of this property, whether the column is resized by the user or programmatically. If the table column’s current width is less than the value of this property, the width is set to the value of this property.

## See Also

### Controlling Size

var width: CGFloat

The table column’s width, in points.

var maxWidth: CGFloat

The table column’s maximum width, in points.

var resizingMask: NSTableColumn.ResizingOptions

The table column’s resizing mask.

func sizeToFit()

Resizes the table column to fit the width of its header cell.

