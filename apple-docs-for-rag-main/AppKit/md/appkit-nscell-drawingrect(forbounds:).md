

- AppKit
- NSCell
-  drawingRect(forBounds:) 

Instance Method

# drawingRect(forBounds:)

Returns the rectangle within which the receiver draws itself

macOS

``` source
@MainActor
func drawingRect(forBounds rect: NSRect) -> NSRect
```

## Parameters 

`rect`  

The bounding rectangle of the receiver.

## Return Value

The rectangle in which the receiver draws itself. This rectangle is slightly inset from the one in `theRect`.

## See Also

### Related Documentation

func calcSize()

Recomputes any internal sizing information for the receiver, if necessary.

Deprecated

### Determining Cell Size

func calcDrawInfo(NSRect)

Recalculates the cell geometry.

var cellSize: NSSize

The minimum size needed to display the cell.

func cellSize(forBounds: NSRect) -> NSSize

Returns the minimum size needed to display the receiver, constraining it to the specified rectangle.

func imageRect(forBounds: NSRect) -> NSRect

Returns the rectangle in which the receiver draws its image.

func titleRect(forBounds: NSRect) -> NSRect

Returns the rectangle in which the receiver draws its title text.

var controlSize: NSControl.ControlSize

The size of the cell.

