

- SwiftUI
- PointerStyle
-  default 

Type Property

# default

The pointer style that uses the default platform appearance.

macOS 15.0+visionOS 2.0+

``` source
static let `default`: PointerStyle
```

## Discussion

This is the default pointer style for interacting with content and UI elements if no other pointer style is more appropriate. This pointer style displays an arrow in macOS and a circle in iPadOS and visionOS.

You might want to set this pointer style explicitly using the pointerStyle(_:) modifier to override another style in the environment.

