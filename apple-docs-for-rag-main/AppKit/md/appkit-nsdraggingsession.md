

- AppKit
-  NSDraggingSession 

Class

# NSDraggingSession

The encapsulation of a drag-and-drop action that supports modification of the drag while in progress.

macOS 10.7+

``` source
class NSDraggingSession
```

## Overview

You start a new dragging session by calling the `NSView` method beginDraggingSession(with:event:source:) method. This method immediately returns and you can further modify the properties of the dragging session. The actual drag begins at the next turn of the run loop.

## Topics

### Dragging Pasteboard

var draggingPasteboard: NSPasteboard

Returns the pasteboard object that contains the data being dragged.

### Dragging Visual Representation

var animatesToStartingPositionsOnCancelOrFail: Bool

Controls whether the dragging image animates back to its starting point on a cancelled or failed drag.

var draggingFormation: NSDraggingFormation

Controls the dragging formation when the drag is not over the source or a valid destination.

### Identifying the Dragging Session

var draggingSequenceNumber: Int

Returns a number that uniquely identifies the dragging session.

### Enumerating Dragging Items

func enumerateDraggingItems(options: NSDraggingItemEnumerationOptions, for: NSView?, classes: [AnyClass], searchOptions: [NSPasteboard.ReadingOptionKey : Any], using: (NSDraggingItem, Int, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates through each dragging item.

### Dragging Session Location

var draggingLocation: NSPoint

The current cursor location of the drag in screen coordinates.

### Dragging Item Location

var draggingLeaderIndex: Int

The index of the dragging item under the cursor.

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

class NSDraggingImageComponent

A single object in a dragging item.

