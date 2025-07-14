

- SwiftUI
- Image
-  Image.TemplateRenderingMode 

Enumeration

# Image.TemplateRenderingMode

A type that indicates how SwiftUI renders images.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum TemplateRenderingMode
```

## Topics

### Getting rendering modes

case original

A mode that renders pixels of bitmap images as-is.

case template

A mode that renders all non-transparent pixels as the foreground color.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Specifying rendering behavior

func antialiased(Bool) -> Image

Specifies whether SwiftUI applies antialiasing when rendering the image.

func symbolRenderingMode(SymbolRenderingMode?) -> Image

Sets the rendering mode for symbol images within this view.

func renderingMode(Image.TemplateRenderingMode?) -> Image

Indicates whether SwiftUI renders an image as-is, or by using a different mode.

func interpolation(Image.Interpolation) -> Image

Specifies the current level of quality for rendering an image that requires interpolation.

enum Interpolation

The level of quality for rendering an image that requires interpolation, such as a scaled image.

