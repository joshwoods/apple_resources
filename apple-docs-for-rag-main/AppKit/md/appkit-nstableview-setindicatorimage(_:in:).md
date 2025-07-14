

- AppKit
- NSTableView
-  setIndicatorImage(\_:in:) 

Instance Method

# setIndicatorImage(\_:in:)

Sets the indicator image of the specified column.

macOS

``` source
@MainActor
func setIndicatorImage(
    _ image: NSImage?,
    in tableColumn: NSTableColumn
)
```

## Parameters 

`image`  

The indicator image for the column.

`tableColumn`  

The table column.

## Discussion

The default sorting order indicators are available as named `NSImage` objects. These images are accessed using `[NSImage imageNamed:]` passing either `@"NSAscendingSortIndicator"` (the “^” icon), and `@"NSDescendingSortIndicator"` (the “v” icon).

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

var gridStyleMask: NSTableView.GridLineStyle

The grid lines drawn by the table view.

func indicatorImage(in: NSTableColumn) -> NSImage?

Returns the indicator image of the specified table column.

