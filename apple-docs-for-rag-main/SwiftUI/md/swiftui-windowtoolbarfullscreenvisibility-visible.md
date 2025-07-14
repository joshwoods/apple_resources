

- SwiftUI
- WindowToolbarFullScreenVisibility
-  visible 

Type Property

# visible

Prefer to show window toolbar when the window is in full screen mode.

macOS 15.0+

``` source
static let visible: WindowToolbarFullScreenVisibility
```

## Discussion

This has no effect if the toolbar is completely hidden, i.e. setting the visibility to `hidden` for `windowToolbar` placements using toolbarVisibility(_:for:) will cause the toolbar to remain completely hidden, even in full screen.

