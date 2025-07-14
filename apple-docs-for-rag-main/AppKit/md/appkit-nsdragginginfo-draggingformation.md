

- AppKit
- NSDraggingInfo
-  draggingFormation 

Instance Property

# draggingFormation

The formation of the dragging items while the drag is over the destination.

macOS 10.7+

``` source
@MainActor
var draggingFormation: NSDraggingFormation { get set }
```

**Required**

## Discussion

Set this property to change the formation of the drag items. This is generally done during the updateDraggingItemsForDrag(_:) method or whenever you enumerate the dragging items.

The default value is the current drag formation.

Note

Set this property before or after the NSDraggingInfo or NSDraggingSession class’s method enumerateDraggingItems(options:for:classes:searchOptions:using:) not inside the enumeration Block.

## See Also

### Sliding the image

func slideDraggedImage(to: NSPoint)

Slides the image to a specified location.

**Required**

var animatesToDestination: Bool

A Boolean value that indicates whether the dragging formation animates while the drag is over the destination.

**Required**

