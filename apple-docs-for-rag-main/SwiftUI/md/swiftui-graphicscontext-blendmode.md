

- SwiftUI
- GraphicsContext
-  blendMode 

Instance Property

# blendMode

The blend mode used by drawing operations in the context.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var blendMode: GraphicsContext.BlendMode { get set }
```

## Discussion

Set this value to affect how any content that you subsequently draw into the context blends with content that’s already in the context. Use one of the GraphicsContext.BlendMode values.

## See Also

### Setting opacity and the blend mode

var opacity: Double

The opacity of drawing operations in the context.

struct BlendMode

The ways that a graphics context combines new content with background content.

