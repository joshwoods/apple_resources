

- SwiftUI
- GraphicsContext
- GraphicsContext.BlendMode
-  multiply 

Type Property

# multiply

A mode that multiplies the source image samples with the background image samples.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var multiply: GraphicsContext.BlendMode { get }
```

## Discussion

Drawing in this mode results in colors that are at least as dark as either of the two contributing sample colors.

## See Also

### Darkening

static var darken: GraphicsContext.BlendMode

A mode that creates composite image samples by choosing the darker samples from either the source image or the background.

static var colorBurn: GraphicsContext.BlendMode

A mode that darkens background image samples to reflect the source image samples.

static var plusDarker: GraphicsContext.BlendMode

A mode that adds the inverse of the color components of the source and background images, and then inverts the result, producing a darkened composite.

