

- AppKit
- NSTableView
-  drawBackground(inClipRect:) 

Instance Method

# drawBackground(inClipRect:)

Draws the background of the table view in the clip rect specified by the rectangle.

macOS

``` source
@MainActor
func drawBackground(inClipRect clipRect: NSRect)
```

## Parameters 

`clipRect`  

The rectangle, in the table view’s coordinate system.

## See Also

### Drawing

func drawRow(Int, clipRect: NSRect)

Draws the cells for the row at `rowIndex` in the columns that intersect `clipRect`.

func drawGrid(inClipRect: NSRect)

Draws the grid lines within the supplied rectangle.

func highlightSelection(inClipRect: NSRect)

Highlights the region of the table view in the specified rectangle.

