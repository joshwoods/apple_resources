

- AppKit
- NSMatrix
-  sizeToCells() 

Instance Method

# sizeToCells()

Changes the width and the height of the receiver’s frame so it exactly contains the cells.

macOS

``` source
@MainActor
func sizeToCells()
```

## Discussion

This method does not redraw the receiver.

## See Also

### Related Documentation

func setFrameSize(NSSize)

Sets the size of the view’s frame rectangle to the specified dimensions, resizing it within its superview without affecting its coordinate system.

func sizeToFit()

Resizes the receiver’s frame so that it’s the minimum size needed to contain its cell.

### Resizing the Matrix and Its Cells

var autosizesCells: Bool

A Boolean that indicates whether the cell sizes change when the receiver is resized.

func setValidateSize(Bool)

Specifies whether the receiver’s size information is validated.

