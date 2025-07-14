

- SwiftUI
- GraphicsContext
- GraphicsContext.BlendMode
-  overlay 

Type Property

# overlay

A mode that either multiplies or screens the source image samples with the background image samples, depending on the background color.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var overlay: GraphicsContext.BlendMode { get }
```

## Discussion

Drawing in this mode overlays the existing image samples while preserving the highlights and shadows of the background. The background color mixes with the source image to reflect the lightness or darkness of the background.

## See Also

### Adding contrast

static var softLight: GraphicsContext.BlendMode

A mode that either darkens or lightens colors, depending on the source image sample color.

static var hardLight: GraphicsContext.BlendMode

A mode that either multiplies or screens colors, depending on the source image sample color.

