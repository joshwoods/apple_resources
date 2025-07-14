

- AppKit
- NSDraggingItem
-  imageComponentsProvider 

Instance Property

# imageComponentsProvider

An array of blocks that provide the dragging image components.

macOS 10.7+

``` source
var imageComponentsProvider: (() -> [NSDraggingImageComponent])? { get set }
```

## Discussion

The dragging image is the composite of an array of NSDraggingImageComponent objects.

The dragging image components aren’t set directly. Instead, use a block to generate the components and the system calls the block if necessary.

You can set the block to `nil`, meaning that the drag item has no image. Generally, only dragging destinations do this, and only if there’s at least one valid item in the drop, and the receiver isn’t that object.

The system arranges the components in painting order. That is, the system paints each component in the array on top of the previous components in the array.

## See Also

### Drag image components

var imageComponents: [NSDraggingImageComponent]?

An array of dragging image components to use to create the drag image.

struct ImageComponentKey

Keys that identify components of a dragging image.

var item: Any

The pasteboard reader or writer object dependent on the context where you use the dragging item.

