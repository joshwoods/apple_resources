

- AppKit
- NSPathCell
-  pathComponentCells 

Instance Property

# pathComponentCells

Sets the array of `NSPathComponentCell` objects currently being displayed.

macOS 10.5+

``` source
@MainActor
var pathComponentCells: [NSPathComponentCell] { get set }
```

## Parameters 

`cells`  

An array of `NSPathComponentCell` objects.

## Discussion

Each item in the array must be an instance of `NSPathComponentCell` or a subclass thereof. You cannot set this value to `nil`, but you can set it to an empty array using, for example, `[NSArray array]`.

## See Also

### Managing Path Components

class var pathComponentCellClass: AnyClass

Returns the class used to create `pathComponentCell` objects when automatically filling up the control.

func rect(of: NSPathComponentCell, withFrame: NSRect, in: NSView) -> NSRect

Returns the current rectangle being displayed for a given path component cell, with respect to a given frame in a given view.

func pathComponentCell(at: NSPoint, withFrame: NSRect, in: NSView) -> NSPathComponentCell?

Returns the cell located at the given point within the given frame of the given view.

var clickedPathComponentCell: NSPathComponentCell?

Sets the value of the path displayed by the receiver.

