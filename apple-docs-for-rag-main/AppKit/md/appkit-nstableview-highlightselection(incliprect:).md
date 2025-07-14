

- AppKit
- NSTableView
-  highlightSelection(inClipRect:) 

Instance Method

# highlightSelection(inClipRect:)

Highlights the region of the table view in the specified rectangle.

macOS

``` source
@MainActor
func highlightSelection(inClipRect clipRect: NSRect)
```

## Parameters 

`clipRect`  

The rectangle, in the table view view’s coordinate system.

## Discussion

This method is invoked before drawRow(_:clipRect:).

NSCell-based table views can override this method to change the manner in which they highlight selections.

Note

This method should not be subclassed or overridden for a view-base table view. Instead, row drawing customization should be done by subclassing NSTableRowView.

## See Also

### Drawing

func drawRow(Int, clipRect: NSRect)

Draws the cells for the row at `rowIndex` in the columns that intersect `clipRect`.

func drawGrid(inClipRect: NSRect)

Draws the grid lines within the supplied rectangle.

func drawBackground(inClipRect: NSRect)

Draws the background of the table view in the clip rect specified by the rectangle.

