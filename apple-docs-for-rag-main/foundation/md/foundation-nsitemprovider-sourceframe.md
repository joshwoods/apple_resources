

- Foundation
- NSItemProvider
-  sourceFrame 

Instance Property

# sourceFrame

The rectangle that the item occupies in the host app’s source window.

macOS 10.10+

``` source
var sourceFrame: NSRect { get }
```

## Discussion

This property contains the rectangle, in screen coordinates, that encloses the item. This rectangle includes areas that might be clipped and not currently visible onscreen.

## See Also

### Getting the provider’s frame

var containerFrame: NSRect

The rectangle of the item’s visible content.

