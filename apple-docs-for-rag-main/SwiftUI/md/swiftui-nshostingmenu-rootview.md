

- SwiftUI
- NSHostingMenu
-  rootView 

Instance Property

# rootView

The root view of the SwiftUI view hierarchy managed by this menu.

macOS 14.4+

``` source
var rootView: Content { get set }
```

## Discussion

Updating this property will immediately update the `items` array, even if the menu is currently visible to the user.

