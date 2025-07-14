

- AppKit
- NSTableView
-  gridStyleMask 

Instance Property

# gridStyleMask

The grid lines drawn by the table view.

macOS

``` source
@MainActor
var gridStyleMask: NSTableView.GridLineStyle { get set }
```

## Discussion

Use this property to specify whether lines should be drawn between rows and columns. When setting this property, you can specify multiple styles at once by adding the corresponding constants together. The default value of this property is NSTableViewGridNone.

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

var selectionHighlightStyle: NSTableView.SelectionHighlightStyle

The selection highlight style used by the table view to indicate row and column selection.

var gridColor: NSColor

The color used to draw grid lines.

func indicatorImage(in: NSTableColumn) -> NSImage?

Returns the indicator image of the specified table column.

func setIndicatorImage(NSImage?, in: NSTableColumn)

Sets the indicator image of the specified column.

