

- AppKit
- NSTableRowView
-  drawSelection(in:) 

Instance Method

# drawSelection(in:)

Draws the selected row.

macOS 10.7+

``` source
@MainActor
func drawSelection(in dirtyRect: NSRect)
```

## Parameters 

`dirtyRect`  

The rectangle that requires drawing.

## Discussion

This method is only called if the selection should be drawn.

The selection will automatically be alpha-blended if the selection is animating in or out.

The default selection drawn is dependent on the selectionHighlightStyle.

## See Also

### Overriding Row View Display Characteristics

var backgroundColor: NSColor

The background color of the row.

func drawBackground(in: NSRect)

Draws the background of the row in the rectangle.

func drawDraggingDestinationFeedback(in: NSRect)

Draws the row’s dragging destination feedback when the entire row is a drop target.

func drawSeparator(in: NSRect)

Draws the horizontal separator between table rows.

