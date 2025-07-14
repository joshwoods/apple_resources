

- AppKit
- NSTableRowView
-  drawBackground(in:) 

Instance Method

# drawBackground(in:)

Draws the background of the row in the rectangle.

macOS 10.7+

``` source
@MainActor
func drawBackground(in dirtyRect: NSRect)
```

## Parameters 

`dirtyRect`  

The rectangle that requires drawing.

## Discussion

Overriding this method allows an application to draw a custom background for a table row view.

By default, this method draws the background color or group row style as appropriate for the row. This method also draws the “below look” for a drop target if isTargetForDropOperation is true.

## See Also

### Overriding Row View Display Characteristics

var backgroundColor: NSColor

The background color of the row.

func drawDraggingDestinationFeedback(in: NSRect)

Draws the row’s dragging destination feedback when the entire row is a drop target.

func drawSelection(in: NSRect)

Draws the selected row.

func drawSeparator(in: NSRect)

Draws the horizontal separator between table rows.

