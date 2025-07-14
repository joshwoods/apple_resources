

- AppKit
- NSTableCellView
-  rowSizeStyle 

Instance Property

# rowSizeStyle

Returns the row size style.

macOS 10.7+

``` source
@MainActor
var rowSizeStyle: NSTableView.RowSizeStyle { get set }
```

## Discussion

The `rowSizeStyle` property is set by the `NSTableView` to its effectiveRowSizeStyle. The cell view will layout the textField and imageView based on the `rowSizeStyle`.

A value of NSTableView.RowSizeStyle.default should never be set on the cell view, as it is an appropriate value only for the table as it returns the effective row size style for the table.

