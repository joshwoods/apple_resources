

- AppKit
- NSPathCell
-  clickedPathComponentCell 

Instance Property

# clickedPathComponentCell

Sets the value of the path displayed by the receiver.

macOS 10.5+

``` source
@MainActor
var clickedPathComponentCell: NSPathComponentCell? { get }
```

## Parameters 

`url`  

The new path value to display.

## Discussion

When setting, an array of `NSPathComponentCell` objects is automatically set, based on the path in `url`. The type of `NSPathComponentCell` objects created can be controlled by subclassing `NSPathCell` and overriding pathComponentCellClass.

If `url` is a file URL (returns true from isFileURL), the images are automatically filled with file icons, if the path exists. The URL value itself is stored in the `objectValue` property of the cell.

## See Also

### Managing Path Components

class var pathComponentCellClass: AnyClass

Returns the class used to create `pathComponentCell` objects when automatically filling up the control.

func rect(of: NSPathComponentCell, withFrame: NSRect, in: NSView) -> NSRect

Returns the current rectangle being displayed for a given path component cell, with respect to a given frame in a given view.

func pathComponentCell(at: NSPoint, withFrame: NSRect, in: NSView) -> NSPathComponentCell?

Returns the cell located at the given point within the given frame of the given view.

var pathComponentCells: [NSPathComponentCell]

Sets the array of `NSPathComponentCell` objects currently being displayed.

