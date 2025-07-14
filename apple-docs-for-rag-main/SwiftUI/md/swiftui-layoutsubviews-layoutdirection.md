

- SwiftUI
- LayoutSubviews
-  layoutDirection 

Instance Property

# layoutDirection

The layout direction inherited by the container view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var layoutDirection: LayoutDirection
```

## Discussion

SwiftUI supports both left-to-right and right-to-left directions. Read this property within a custom layout container to find out which environment the container is in.

In most cases, you don’t need to take any action based on this value. SwiftUI horizontally flips the x position of each view within its parent when the mode switches, so layout calculations automatically produce the desired effect for both directions.

