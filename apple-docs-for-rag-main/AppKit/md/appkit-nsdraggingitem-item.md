

- AppKit
- NSDraggingItem
-  item 

Instance Property

# item

The pasteboard reader or writer object dependent on the context where you use the dragging item.

macOS 10.7+

``` source
var item: Any { get }
```

## Discussion

When you create an `NSDraggingItem` instance, `item` is the `pasteboardWriter` passed to init(pasteboardWriter:).

However, when enumerating dragging items using the NSDraggingSession method enumerateDraggingItems(options:for:classes:searchOptions:using:) or the NSDraggingInfo method enumerateDraggingItems(options:for:classes:searchOptions:using:), `item` is not the original pasteboard reader or writer instance. It is an instance of one of the classes provided to the enumeration method’s `classArray` parameter.

## See Also

### Drag image components

var imageComponents: [NSDraggingImageComponent]?

An array of dragging image components to use to create the drag image.

var imageComponentsProvider: (() -> [NSDraggingImageComponent])?

An array of blocks that provide the dragging image components.

struct ImageComponentKey

Keys that identify components of a dragging image.

