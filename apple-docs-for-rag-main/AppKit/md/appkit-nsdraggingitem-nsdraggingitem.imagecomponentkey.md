

- AppKit
- NSDraggingItem
-  NSDraggingItem.ImageComponentKey 

Structure

# NSDraggingItem.ImageComponentKey

Keys that identify components of a dragging image.

macOS

``` source
struct ImageComponentKey
```

## Topics

### Initializing a component key

init(String)

Creates an image component key using the string you provide.

init(rawValue: String)

Creates an image component key using the string you provide.

### Image component keys

static let icon: NSDraggingItem.ImageComponentKey

A key for a corresponding value that is a dragging item’s image.

static let label: NSDraggingItem.ImageComponentKey

A key for a corresponding value that represents a textual label for a dragging item, for example, a file name.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Drag image components

var imageComponents: [NSDraggingImageComponent]?

An array of dragging image components to use to create the drag image.

var imageComponentsProvider: (() -> [NSDraggingImageComponent])?

An array of blocks that provide the dragging image components.

var item: Any

The pasteboard reader or writer object dependent on the context where you use the dragging item.

