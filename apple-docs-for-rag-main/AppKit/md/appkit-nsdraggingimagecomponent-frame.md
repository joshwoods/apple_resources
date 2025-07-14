

- AppKit
- NSDraggingImageComponent
-  frame 

Instance Property

# frame

The coordinate space is the bounds of the parent dragging item.

macOS 10.7+

``` source
var frame: NSRect { get set }
```

## Discussion

The frame is {{0,0}, {`draggingFrame.size.width`, `draggingFrame.size.height`}}.

The coordinate space is the bounds of the parent NSDraggingItem instance’s draggingFrame.

## See Also

### Related Documentation

var draggingFrame: NSRect

The frame of the dragging item.

### Dragging Image Contents

var contents: Any?

An object providing the image contents of the component.

