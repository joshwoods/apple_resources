

- AppKit
- NSPathCell
-  pathComponentCellClass 

Type Property

# pathComponentCellClass

Returns the class used to create `pathComponentCell` objects when automatically filling up the control.

macOS 10.5+

``` source
@MainActor
class var pathComponentCellClass: AnyClass { get }
```

## Return Value

The class used to create `NSPathComponentCell` objects.

## Discussion

Subclasses can override this method to return a custom cell class that is automatically used. By default, the method returns `[NSPathComponentCell class]`, or a specialized subclass thereof.

## See Also

### Managing Path Components

func rect(of: NSPathComponentCell, withFrame: NSRect, in: NSView) -> NSRect

Returns the current rectangle being displayed for a given path component cell, with respect to a given frame in a given view.

func pathComponentCell(at: NSPoint, withFrame: NSRect, in: NSView) -> NSPathComponentCell?

Returns the cell located at the given point within the given frame of the given view.

var clickedPathComponentCell: NSPathComponentCell?

Sets the value of the path displayed by the receiver.

var pathComponentCells: [NSPathComponentCell]

Sets the array of `NSPathComponentCell` objects currently being displayed.

