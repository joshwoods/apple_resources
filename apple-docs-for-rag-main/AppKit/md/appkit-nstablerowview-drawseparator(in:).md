

- AppKit
- NSTableRowView
-  drawSeparator(in:) 

Instance Method

# drawSeparator(in:)

Draws the horizontal separator between table rows.

macOS 10.7+

``` source
@MainActor
func drawSeparator(in dirtyRect: NSRect)
```

## Parameters 

`dirtyRect`  

The rectangle that requires drawing.

## Discussion

By default, the separator is only drawn if the enclosing table’s gridStyleMask is set to include a horizontal separator.

The separator should be drawn at the bottom of the row view, indicating a separation from this row and the next.

## See Also

### Overriding Row View Display Characteristics

var backgroundColor: NSColor

The background color of the row.

func drawBackground(in: NSRect)

Draws the background of the row in the rectangle.

func drawDraggingDestinationFeedback(in: NSRect)

Draws the row’s dragging destination feedback when the entire row is a drop target.

func drawSelection(in: NSRect)

Draws the selected row.

