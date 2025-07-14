

- AppKit
- NSCell
-  titleRect(forBounds:) 

Instance Method

# titleRect(forBounds:)

Returns the rectangle in which the receiver draws its title text.

macOS

``` source
@MainActor
func titleRect(forBounds rect: NSRect) -> NSRect
```

## Parameters 

`rect`  

The bounding rectangle of the receiver.

## Return Value

The rectangle in which the receiver draws its title text.

## Discussion

If the receiver is a text-type cell, this method resizes the drawing rectangle for the title (`theRect`) inward by a small offset to accommodate the cell border. If the receiver is not a text-type cell, the method does nothing.

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

func imageRect(forBounds: NSRect) -> NSRect

Returns the rectangle in which the receiver draws its image.

var controlSize: NSControl.ControlSize

The size of the cell.

