

- AppKit
- NSDraggingItem
-  init(pasteboardWriter:) 

Initializer

# init(pasteboardWriter:)

Creates and returns a dragging item using the specified content.

macOS 10.7+

``` source
init(pasteboardWriter: any NSPasteboardWriting)
```

## Parameters 

`pasteboardWriter`  

The object that provides the dragging content. The object must implement the NSPasteboardWriting protocol.

## Return Value

An initialized NSDraggingItem instance with the specified dragging content.

## Discussion

When the developer creates an `NSDraggingItem` instance , it is for use with the view method beginDraggingSession(with:event:source:) During the invocation of that method, the `pasteboardWriter` is placed onto the dragging pasteboard for the `NSDraggingSession` that contains the dragging item instance.

The designated initializer.

