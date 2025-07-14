

- AppKit
- NSPathControlDelegate
-  pathControl(\_:shouldDrag:with:) 

Instance Method

# pathControl(\_:shouldDrag:with:)

Implement this method to enable dragging from the control.

macOS 10.5+

``` source
@MainActor
optional func pathControl(
    _ pathControl: NSPathControl,
    shouldDrag pathComponentCell: NSPathComponentCell,
    with pasteboard: NSPasteboard
) -> Bool
```

## Parameters 

`pathControl`  

The path control that sent the message.

`pathComponentCell`  

The path component cell from which the drag is beginning.

`pasteboard`  

The pasteboard.

## Discussion

This method is called when a drag is about to begin. You can refuse to allow the drag to happen by returning false and allow it by returning true. By default, the pasteboard automatically has the following types on it: `NSStringPboardType`, `NSURLPboardType` (if there is a URL value for the cell being dragged), and `NSFilenamesPboardType` (if the URL value returns true from -isFileURL). You can customize the types placed on the pasteboard at this time, if desired. Implementation of this method is optional.

## See Also

### Dragging Support

func pathControl(NSPathControl, validateDrop: any NSDraggingInfo) -> NSDragOperation

Implement this method to enable dragging onto the control.

func pathControl(NSPathControl, acceptDrop: any NSDraggingInfo) -> Bool

Implement this method to accept previously validated contents dropped onto the control.

