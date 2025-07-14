

- AppKit
-  NSDraggingItem 

Class

# NSDraggingItem

A single dragged item within a dragging session.

macOS 10.7+

``` source
class NSDraggingItem
```

## Overview

NSDraggingItem objects have extremely limited lifetimes. Don’t retain these items because changing outside of the prescribed lifetimes has no impact on the drag.

When you call the NSDraggingSession method beginDraggingSession(with:event:source:), the system immediately consumes the dragging items that pass to the method, and doesn’t retain them. Any further changes to the dragging item associated with the returned NSDraggingSession must occur with the enumeration method enumerateDraggingItems(options:for:classes:searchOptions:using:). When enumerating, the system creates `NSDraggingItem` instances right before giving them to the enumeration block. After returning from the block, the dragging item is no longer valid.

## Topics

### Initializing a dragging item

init(pasteboardWriter: any NSPasteboardWriting)

Creates and returns a dragging item using the specified content.

### Dragging frame

func setDraggingFrame(NSRect, contents: Any?)

Sets the item’s dragging frame and contents.

var draggingFrame: NSRect

The frame of the dragging item.

### Drag image components

var imageComponents: [NSDraggingImageComponent]?

An array of dragging image components to use to create the drag image.

var imageComponentsProvider: (() -> [NSDraggingImageComponent])?

An array of blocks that provide the dragging image components.

struct ImageComponentKey

Keys that identify components of a dragging image.

var item: Any

The pasteboard reader or writer object dependent on the context where you use the dragging item.

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

class NSDraggingSession

The encapsulation of a drag-and-drop action that supports modification of the drag while in progress.

class NSDraggingImageComponent

A single object in a dragging item.

