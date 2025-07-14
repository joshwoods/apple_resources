

- AppKit
- NSTableCellView
-  draggingImageComponents 

Instance Property

# draggingImageComponents

Returns dragging images for the cell.

macOS 10.7+

``` source
@MainActor
var draggingImageComponents: [NSDraggingImageComponent] { get }
```

## Discussion

The default implementation of this method returns an array of up to two `NSDraggingImageComponent` instances – one for the imageView and another for the textField (unless the property is `nil`).

These method can be subclassed and overridden to provide a custom set of `NSDraggingImageComponent` objects to create the drag image from this view.

