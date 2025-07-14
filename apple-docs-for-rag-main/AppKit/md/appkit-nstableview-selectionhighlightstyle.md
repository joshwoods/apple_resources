

- AppKit
- NSTableView
-  selectionHighlightStyle 

Instance Property

# selectionHighlightStyle

The selection highlight style used by the table view to indicate row and column selection.

macOS 10.5+

``` source
@MainActor
var selectionHighlightStyle: NSTableView.SelectionHighlightStyle { get set }
```

## Discussion

Setting the selection highlight style to NSTableView.SelectionHighlightStyle.sourceList causes the table view to draw its background using the source list style. It also sets the draggingDestinationFeedbackStyle to NSTableView.DraggingDestinationFeedbackStyle.sourceList.

## See Also

### Setting Display Attributes

var intercellSpacing: NSSize

The horizontal and vertical spacing between cells.

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

var gridColor: NSColor

The color used to draw grid lines.

var gridStyleMask: NSTableView.GridLineStyle

The grid lines drawn by the table view.

func indicatorImage(in: NSTableColumn) -> NSImage?

Returns the indicator image of the specified table column.

func setIndicatorImage(NSImage?, in: NSTableColumn)

Sets the indicator image of the specified column.

