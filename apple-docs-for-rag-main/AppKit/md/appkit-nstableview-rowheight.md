

- AppKit
- NSTableView
-  rowHeight 

Instance Property

# rowHeight

The height of each row in the table.

macOS

``` source
@MainActor
var rowHeight: CGFloat { get set }
```

## Discussion

The default row height is `16.0`. The value in this property is used only if the table’s rowSizeStyle is set to NSTableView.RowSizeStyle.custom.

When you change the value of this property, the table view calls the tile() method to redisplay the rows using the new value.

## See Also

### Related Documentation

var rowSizeStyle: NSTableView.RowSizeStyle

The row size style (small, medium, large, or custom) used by the table view.

### Setting Display Attributes

var intercellSpacing: NSSize

The horizontal and vertical spacing between cells.

var backgroundColor: NSColor

The color used to draw the background of the table.

var usesAlternatingRowBackgroundColors: Bool

A Boolean value indicating whether the table view uses alternating row colors for its background.

var style: NSTableView.Style

The style that the table view uses.

var effectiveStyle: NSTableView.Style

The effective style that the table uses.

enum Style

Contains the possible style values for a table view.

var selectionHighlightStyle: NSTableView.SelectionHighlightStyle

The selection highlight style used by the table view to indicate row and column selection.

var gridColor: NSColor

The color used to draw grid lines.

var gridStyleMask: NSTableView.GridLineStyle

The grid lines drawn by the table view.

func indicatorImage(in: NSTableColumn) -> NSImage?

Returns the indicator image of the specified table column.

func setIndicatorImage(NSImage?, in: NSTableColumn)

Sets the indicator image of the specified column.

