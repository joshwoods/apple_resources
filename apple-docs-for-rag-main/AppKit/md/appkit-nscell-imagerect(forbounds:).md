

- AppKit
- NSCell
-  imageRect(forBounds:) 

Instance Method

# imageRect(forBounds:)

Returns the rectangle in which the receiver draws its image.

macOS

``` source
@MainActor
func imageRect(forBounds rect: NSRect) -> NSRect
```

## Parameters 

`rect`  

The bounding rectangle of the receiver.

## Return Value

The rectangle in which the receiver draws its image. This rectangle is slightly offset from the one in `theRect`.

## See Also

### Determining Cell Size

func calcDrawInfo(NSRect)

Recalculates the cell geometry.

var cellSize: NSSize

The minimum size needed to display the cell.

func cellSize(forBounds: NSRect) -> NSSize

Returns the minimum size needed to display the receiver, constraining it to the specified rectangle.

func drawingRect(forBounds: NSRect) -> NSRect

Returns the rectangle within which the receiver draws itself

func titleRect(forBounds: NSRect) -> NSRect

Returns the rectangle in which the receiver draws its title text.

var controlSize: NSControl.ControlSize

The size of the cell.

