

- SwiftUI
- GraphicsContext
- GraphicsContext.ClipOptions
-  inverse 

Type Property

# inverse

An option to invert the shape or layer alpha as the clip mask.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var inverse: GraphicsContext.ClipOptions { get }
```

## Discussion

When you use this option, SwiftUI uses `1 - alpha` instead of `alpha` for the given clip shape.

