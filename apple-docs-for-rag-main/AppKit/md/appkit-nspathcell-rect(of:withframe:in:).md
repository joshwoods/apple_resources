

- AppKit
- NSPathCell
-  rect(of:withFrame:in:) 

Instance Method

# rect(of:withFrame:in:)

Returns the current rectangle being displayed for a given path component cell, with respect to a given frame in a given view.

macOS 10.5+

``` source
@MainActor
func rect(
    of cell: NSPathComponentCell,
    withFrame frame: NSRect,
    in view: NSView
) -> NSRect
```

## Parameters 

`cell`  

The path component cell.

`frame`  

The frame of the view in which the cell appears.

`view`  

The view in which the cell appears.

## Return Value

The rectangle occupied by the path component cell. `NSZeroRect` is returned if `cell` is not found or is not currently visible.

## See Also

### Managing Path Components

class var pathComponentCellClass: AnyClass

Returns the class used to create `pathComponentCell` objects when automatically filling up the control.

func pathComponentCell(at: NSPoint, withFrame: NSRect, in: NSView) -> NSPathComponentCell?

Returns the cell located at the given point within the given frame of the given view.

var clickedPathComponentCell: NSPathComponentCell?

Sets the value of the path displayed by the receiver.

var pathComponentCells: [NSPathComponentCell]

Sets the array of `NSPathComponentCell` objects currently being displayed.

