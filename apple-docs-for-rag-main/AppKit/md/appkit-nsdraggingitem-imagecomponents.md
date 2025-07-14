

- AppKit
- NSDraggingItem
-  imageComponents 

Instance Property

# imageComponents

An array of dragging image components to use to create the drag image.

macOS 10.7+

``` source
var imageComponents: [NSDraggingImageComponent]? { get }
```

## Discussion

The array contains copies of the components. The drag does not reflect changes you make to these copies. If needed, the system calls the imageComponentsProvider block to generate the image components.

## See Also

### Drag image components

var imageComponentsProvider: (() -> [NSDraggingImageComponent])?

An array of blocks that provide the dragging image components.

struct ImageComponentKey

Keys that identify components of a dragging image.

var item: Any

The pasteboard reader or writer object dependent on the context where you use the dragging item.

