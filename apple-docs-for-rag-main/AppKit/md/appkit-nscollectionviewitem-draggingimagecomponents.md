

- AppKit
- NSCollectionViewItem
-  draggingImageComponents 

Instance Property

# draggingImageComponents

Dragging images for multi-image drag and drop support.

macOS 10.7+

``` source
@MainActor
var draggingImageComponents: [NSDraggingImageComponent] { get }
```

## Discussion

The component frames are relative to a coordinate system that has its origin at the bottom left, so you need to take into account the flipped state of your view when computing the component frames.

This methods can be subclassed and overridden to provide a custom set of NSDraggingImageComponent objects to create the drag image.

The default implementation will return an array of up to two NSDraggingImageComponent instances – one for the imageView and another for the textField (if not `nil`).

