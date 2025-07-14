

- AppKit
- NSDraggingInfo
-  draggedImageLocation 

Instance Property

# draggedImageLocation

The current location of the dragged image’s origin, in the base coordinate system of the destination object’s window.

macOS

``` source
@MainActor
var draggedImageLocation: NSPoint { get }
```

**Required**

## Discussion

The image moves along with the mouse pointer (the position of which is given by draggingLocation) but may be positioned at some offset.

## See Also

### Getting image information

var draggedImage: NSImage?

The image that represents the dragging item.

**Required**

Deprecated

