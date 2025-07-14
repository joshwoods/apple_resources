

- AppKit
-  NSPathControlDelegate 

Protocol

# NSPathControlDelegate

A set of methods that can be implemented by the delegate of a path control object to support dragging to and from the control.

macOS

``` source
protocol NSPathControlDelegate : NSObjectProtocol
```

## Topics

### Dragging Support

func pathControl(NSPathControl, shouldDrag: NSPathComponentCell, with: NSPasteboard) -> Bool

Implement this method to enable dragging from the control.

func pathControl(NSPathControl, validateDrop: any NSDraggingInfo) -> NSDragOperation

Implement this method to enable dragging onto the control.

func pathControl(NSPathControl, acceptDrop: any NSDraggingInfo) -> Bool

Implement this method to accept previously validated contents dropped onto the control.

### Customizing a Pop-Up–Style Path

func pathControl(NSPathControl, willDisplay: NSOpenPanel)

Implement this method to customize the Open panel shown by a pop-up–style path.

func pathControl(NSPathControl, willPopUp: NSMenu)

Implement this method to customize the menu of a pop-up–style path.

### Instance Methods

func pathControl(NSPathControl, shouldDrag: NSPathControlItem, with: NSPasteboard) -> Bool

## Relationships

### Inherits From

- NSObjectProtocol

