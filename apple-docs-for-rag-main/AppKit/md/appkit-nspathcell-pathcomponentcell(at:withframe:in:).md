

- AppKit
- NSPathCell
-  pathComponentCell(at:withFrame:in:) 

Instance Method

# pathComponentCell(at:withFrame:in:)

Returns the cell located at the given point within the given frame of the given view.

macOS 10.5+

``` source
@MainActor
func pathComponentCell(
    at point: NSPoint,
    withFrame frame: NSRect,
    in view: NSView
) -> NSPathComponentCell?
```

## Parameters 

`point`  

The point within the returned cell.

`frame`  

The frame within which the point is located.

`view`  

The view within which the frame is located.

## Return Value

The component cell within which the given point is located, or `nil` if no cell exists at that location.

## See Also

### Managing Path Components

class var pathComponentCellClass: AnyClass

Returns the class used to create `pathComponentCell` objects when automatically filling up the control.

func rect(of: NSPathComponentCell, withFrame: NSRect, in: NSView) -> NSRect

Returns the current rectangle being displayed for a given path component cell, with respect to a given frame in a given view.

var clickedPathComponentCell: NSPathComponentCell?

Sets the value of the path displayed by the receiver.

var pathComponentCells: [NSPathComponentCell]

Sets the array of `NSPathComponentCell` objects currently being displayed.

