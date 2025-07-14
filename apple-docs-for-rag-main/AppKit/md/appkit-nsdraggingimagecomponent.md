

- AppKit
-  NSDraggingImageComponent 

Class

# NSDraggingImageComponent

A single object in a dragging item.

macOS 10.7+

``` source
class NSDraggingImageComponent
```

## Overview

An array of NSDraggingImageComponent instances are composited together to create the dragging image for an NSDraggingItem. NSDraggingImageComponent instances can simply be considered as named images with a location used by an NSDraggingItem instance.

## Topics

### Creating a Dragging Image Component

init(key: NSDraggingItem.ImageComponentKey)

Initializes and returns a dragging image component with the specified key.

### Dragging Image Component

var key: NSDraggingItem.ImageComponentKey

The unique name of this image component instance.

### Dragging Image Contents

var contents: Any?

An object providing the image contents of the component.

var frame: NSRect

The coordinate space is the bounds of the parent dragging item.

### Constants

NSDragImage Component Keys

These constants are used by the init(key:), draggingImageComponentWithKey: methods and the key property.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Drag Sources

protocol NSDraggingSource

A set of methods that are implemented by the source object in a dragging session.

class NSDraggingItem

A single dragged item within a dragging session.

class NSDraggingSession

The encapsulation of a drag-and-drop action that supports modification of the drag while in progress.

