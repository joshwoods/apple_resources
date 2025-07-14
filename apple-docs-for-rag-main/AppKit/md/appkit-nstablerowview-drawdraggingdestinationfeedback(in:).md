

- AppKit
- NSTableRowView
-  drawDraggingDestinationFeedback(in:) 

Instance Method

# drawDraggingDestinationFeedback(in:)

Draws the row’s dragging destination feedback when the entire row is a drop target.

macOS 10.7+

``` source
@MainActor
func drawDraggingDestinationFeedback(in dirtyRect: NSRect)
```

## Parameters 

`dirtyRect`  

The rectangle that requires drawing.

## Discussion

Overriding this method allows an application to draw custom dragging destination feedback when the entire row is a drop target.

This method only is called if isTargetForDropOperation is true, and is only drawn based on the properties set, such as the group row style.

## See Also

### Overriding Row View Display Characteristics

var backgroundColor: NSColor

The background color of the row.

func drawBackground(in: NSRect)

Draws the background of the row in the rectangle.

func drawSelection(in: NSRect)

Draws the selected row.

func drawSeparator(in: NSRect)

Draws the horizontal separator between table rows.

