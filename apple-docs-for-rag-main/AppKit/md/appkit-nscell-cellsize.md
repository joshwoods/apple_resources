

- AppKit
- NSCell
-  cellSize 

Instance Property

# cellSize

The minimum size needed to display the cell.

macOS

``` source
@MainActor
var cellSize: NSSize { get }
```

## Discussion

This property contains the smallest cell size (in points) required to draw its contents. If the cell is not a text or image cell, the cell size is set to (`10000`, `10000`). If an image cell does not yet have an associated image, the cell size is NSZeroSize.This method takes into account of the size of the image or text in the cell along with any margin areas required by the cell’s border, if any.

## See Also

### Determining Cell Size

func calcDrawInfo(NSRect)

Recalculates the cell geometry.

func cellSize(forBounds: NSRect) -> NSSize

Returns the minimum size needed to display the receiver, constraining it to the specified rectangle.

func drawingRect(forBounds: NSRect) -> NSRect

Returns the rectangle within which the receiver draws itself

func imageRect(forBounds: NSRect) -> NSRect

Returns the rectangle in which the receiver draws its image.

func titleRect(forBounds: NSRect) -> NSRect

Returns the rectangle in which the receiver draws its title text.

var controlSize: NSControl.ControlSize

The size of the cell.

