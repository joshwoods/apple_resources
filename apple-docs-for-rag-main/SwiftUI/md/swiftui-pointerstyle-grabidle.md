

- SwiftUI
- PointerStyle
-  grabIdle 

Type Property

# grabIdle

The pointer style appropriate to indicate that dragging to reposition content within specific bounds, such as panning a large image, is possible.

macOS 15.0+

``` source
static let grabIdle: PointerStyle
```

## Discussion

This pointer style displays an open hand to indicate that the content can be repositioned. Typically it’s used along with the `PointerStyle.grabActive` pointer style while a mouse or trackpad is actively clicked to indicate that the content is currently being repositioned.

You may apply this pointer style to a single view or a view hierarchy using the pointerStyle(_:) modifier.

