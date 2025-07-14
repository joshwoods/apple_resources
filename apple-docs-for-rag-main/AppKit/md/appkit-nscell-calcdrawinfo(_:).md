

- AppKit
- NSCell
-  calcDrawInfo(\_:) 

Instance Method

# calcDrawInfo(\_:)

Recalculates the cell geometry.

macOS

``` source
@MainActor
func calcDrawInfo(_ rect: NSRect)
```

## Parameters 

`rect`  

The reference rectangle to use when calculating the cell information.

## Discussion

Objects (such as controls) that manage `NSCell` objects generally maintain a flag that informs them if any of their cells have been modified in such a way that the location or size of the cell should be recomputed. If so, calcSize() method of `NSControl` is automatically invoked prior to the display of the cell, and that method invokes the calcDrawInfo(_:) method of the cell.

The default implementation of this method does nothing.

## See Also

### Determining Cell Size

var cellSize: NSSize

The minimum size needed to display the cell.

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

