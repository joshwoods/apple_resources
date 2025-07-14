

- SwiftUI
- GraphicsContext
- GraphicsContext.BlendMode
-  luminosity 

Type Property

# luminosity

A mode that uses the hue and saturation of the background with the luminance of the source image.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var luminosity: GraphicsContext.BlendMode { get }
```

## Discussion

This mode creates an effect that is inverse to the effect created by the color mode.

## See Also

### Mixing color components

static var hue: GraphicsContext.BlendMode

A mode that uses the luminance and saturation values of the background with the hue of the source image.

static var saturation: GraphicsContext.BlendMode

A mode that uses the luminance and hue values of the background with the saturation of the source image.

static var color: GraphicsContext.BlendMode

A mode that uses the luminance values of the background with the hue and saturation values of the source image.

