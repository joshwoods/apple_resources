

- AppKit
- NSDraggingItem
-  setDraggingFrame(\_:contents:) 

Instance Method

# setDraggingFrame(\_:contents:)

Sets the item’s dragging frame and contents.

macOS 10.7+

``` source
func setDraggingFrame(
    _ frame: NSRect,
    contents: Any?
)
```

## Parameters 

`frame`  

The item content frame, which is in the same coordinate space as the value of draggingFrame.

`contents`  

The item contents to display when dragging. Typically this is an `NSImage`, but a `CGImageRef` will also work.

## Discussion

Alternate single image component setter.

This convenience method simplifies modifying the components of an `NSDraggingItem` when there is only one component. It sets the draggingFrame and creates a single NSDraggingImageComponent instance with one image corresponding to the icon key. You should use this method only under the following conditions: the drag image for this item is composed of a single image, or there are a reasonable number of dragging item instances being created or enumerated.

If your application requires the dragging of hundreds of items this method would create a instance for each item when it is called. Compare this to the imageComponentsProvider block which is much faster to define and allows AppKit to create only a subset of the items using imageComponentsProvider.

This method sets the draggingFrame and imageComponents properties.

## See Also

### Related Documentation

var imageComponentsProvider: (() -> [NSDraggingImageComponent])?

An array of blocks that provide the dragging image components.

### Dragging frame

var draggingFrame: NSRect

The frame of the dragging item.

