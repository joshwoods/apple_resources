

- SwiftUI
- DisplayProxy
-  safeAreaInsets 

Instance Property

# safeAreaInsets

The safe area inset of this display.

macOS 15.0+

``` source
let safeAreaInsets: EdgeInsets
```

## Discussion

On macOS, the safe area contains space occupied by the dock and menu bar, and is dependent on the current user settings. Additionally, on Macs that include a camera housing in the bezel, the safe area contains the vertical space occupied by the bezel.

