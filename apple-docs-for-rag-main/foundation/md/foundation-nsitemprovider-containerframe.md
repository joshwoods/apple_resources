

- Foundation
- NSItemProvider
-  containerFrame 

Instance Property

# containerFrame

The rectangle of the item’s visible content.

macOS 10.10+

``` source
var containerFrame: NSRect { get }
```

## Discussion

The rectangle in this property corresponds to the onscreen frame rectangle of the item. This rectangle may or may not intersect the sourceFrame rectangle of the item. An intersection of the rectangles means that at least part of the item is visible onscreen.

The rectangle in this property may be a clipped version of the source frame or it might be NSZeroRect if the item is offscreen or the system can’t determine the clipping rectangle. The system treats a value of NSZeroRect as meaning the item is fully visible.

## See Also

### Getting the provider’s frame

var sourceFrame: NSRect

The rectangle that the item occupies in the host app’s source window.

