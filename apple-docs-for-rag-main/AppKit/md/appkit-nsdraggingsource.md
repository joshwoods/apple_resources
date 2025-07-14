

- AppKit
-  NSDraggingSource 

Protocol

# NSDraggingSource

A set of methods that are implemented by the source object in a dragging session.

macOS

``` source
protocol NSDraggingSource : NSObjectProtocol
```

## Overview

In macOS 10.7 and later `NSDraggingSource` is now a formal protocol and has an updated interface. The OS X v10.6 behavior has been retained, but will be dropped in a future version of the operating system. The methods that are to be deprecated are marked as such.

## Topics

### Dragging Session Operation

func draggingSession(NSDraggingSession, sourceOperationMaskFor: NSDraggingContext) -> NSDragOperation

Declares the types of operations the source allows to be performed.

**Required**

### Dragging Session Locations

func draggingSession(NSDraggingSession, willBeginAt: NSPoint)

Invoked when the drag will begin.

func draggingSession(NSDraggingSession, movedTo: NSPoint)

Invoked when the drag moves on the screen.

func draggingSession(NSDraggingSession, endedAt: NSPoint, operation: NSDragOperation)

Invoked when the dragging session has completed.

### Dragging Session Modifier Keys

func ignoreModifierKeys(for: NSDraggingSession) -> Bool

Returns whether the modifier keys will be ignored for this dragging session.

### Dragging Options

func namesOfPromisedFilesDropped(atDestination dropDestination: URL) -> [String]?

Returns the names of the files that the receiver promises to create at a specified location.

Deprecated

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- NSCollectionView
- NSOutlineView
- NSTableView
- NSTextView

## See Also

### Related Documentation

Drag and Drop Programming Topics

### Drag Sources

class NSDraggingItem

A single dragged item within a dragging session.

class NSDraggingSession

The encapsulation of a drag-and-drop action that supports modification of the drag while in progress.

class NSDraggingImageComponent

A single object in a dragging item.

