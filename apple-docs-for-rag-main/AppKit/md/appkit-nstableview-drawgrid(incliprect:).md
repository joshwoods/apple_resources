

- AppKit
- NSTableView
-  drawGrid(inClipRect:) 

Instance Method

# drawGrid(inClipRect:)

Draws the grid lines within the supplied rectangle.

macOS

``` source
@MainActor
func drawGrid(inClipRect clipRect: NSRect)
```

## Parameters 

`clipRect`  

The rectangle in the table view’s coordinate system.

## Discussion

Draws the grid lines within `clipRect`, using the grid color set with gridColor.

Subclasses can override this method to draw grid lines other than the standard ones. This method draws a grid regardless of whether the table view is set to draw one automatically.

## See Also

### Related Documentation

var intercellSpacing: NSSize

The horizontal and vertical spacing between cells.

var gridColor: NSColor

The color used to draw grid lines.

### Drawing

func drawRow(Int, clipRect: NSRect)

Draws the cells for the row at `rowIndex` in the columns that intersect `clipRect`.

func highlightSelection(inClipRect: NSRect)

Highlights the region of the table view in the specified rectangle.

func drawBackground(inClipRect: NSRect)

Draws the background of the table view in the clip rect specified by the rectangle.

