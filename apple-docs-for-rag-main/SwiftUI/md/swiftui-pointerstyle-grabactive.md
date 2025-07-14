

- SwiftUI
- PointerStyle
-  grabActive 

Type Property

# grabActive

The pointer style appropriate for actively dragging to reposition content within specific bounds, such as panning a large image.

macOS 15.0+

``` source
static let grabActive: PointerStyle
```

## Discussion

This pointer style displays a closed hand to indicate that the content is currently being repositioned. Typically it’s used along with the `PointerStyle.grabIdle` pointer style to indicate that repositioning the content is possible.

You may apply this pointer style to a single view or a view hierarchy using the pointerStyle(_:) modifier.

