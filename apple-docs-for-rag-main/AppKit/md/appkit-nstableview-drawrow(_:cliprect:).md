

- AppKit
- NSTableView
-  drawRow(\_:clipRect:) 

Instance Method

# drawRow(\_:clipRect:)

Draws the cells for the row at `rowIndex` in the columns that intersect `clipRect`.

macOS

``` source
@MainActor
func drawRow(
    _ row: Int,
    clipRect: NSRect
)
```

## Parameters 

`row`  

The row index.

`clipRect`  

The intersecting rectangle.

## Discussion

NSCell-based table views can override this method to customize the drawing of the rows.

Note

For NSView-based table views, do not subclass or override this method. Instead, row drawing customization should be done by subclassing NSTableRowView.

## See Also

### Drawing

func drawGrid(inClipRect: NSRect)

Draws the grid lines within the supplied rectangle.

func highlightSelection(inClipRect: NSRect)

Highlights the region of the table view in the specified rectangle.

func drawBackground(inClipRect: NSRect)

Draws the background of the table view in the clip rect specified by the rectangle.

