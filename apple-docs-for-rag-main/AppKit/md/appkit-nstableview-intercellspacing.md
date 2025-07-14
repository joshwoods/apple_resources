

- AppKit
- NSTableView
-  intercellSpacing 

Instance Property

# intercellSpacing

The horizontal and vertical spacing between cells.

macOS

``` source
@MainActor
var intercellSpacing: NSSize { get set }
```

## Discussion

Changing the value of this property causes the table view to redisplay itself. Negative values aren’t supported. The default spacing varies based on the table’s style.

Table views normally have a 1-pixel separation between consecutively selected rows or columns. An intercell spacing of `(1.0, 1.0)` or greater is required if you want this separation. An intercell spacing of `(0.0, 0.0)` forces no separation between consecutive selections.

## See Also

### Setting Display Attributes

var rowHeight: CGFloat

The height of each row in the table.

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

