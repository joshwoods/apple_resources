

- AppKit
- NSTableView
-  indicatorImage(in:) 

Instance Method

# indicatorImage(in:)

Returns the indicator image of the specified table column.

macOS

``` source
@MainActor
func indicatorImage(in tableColumn: NSTableColumn) -> NSImage?
```

## Parameters 

`tableColumn`  

A table column in the table view.

## Discussion

An indicator image is an arbitrary (small) image that is rendered on the right side of the column header. An example of its use is in Mail to indicate the sorting direction of the currently sorted column in a mailbox.

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

func setIndicatorImage(NSImage?, in: NSTableColumn)

Sets the indicator image of the specified column.

