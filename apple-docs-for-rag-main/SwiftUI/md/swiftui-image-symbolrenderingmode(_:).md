

- SwiftUI
- Image
-  symbolRenderingMode(\_:) 

Instance Method

# symbolRenderingMode(\_:)

Sets the rendering mode for symbol images within this view.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func symbolRenderingMode(_ mode: SymbolRenderingMode?) -> Image
```

## Parameters 

`mode`  

The symbol rendering mode to use.

## Return Value

A view that uses the rendering mode you supply.

## See Also

### Specifying rendering behavior

func antialiased(Bool) -> Image

Specifies whether SwiftUI applies antialiasing when rendering the image.

func renderingMode(Image.TemplateRenderingMode?) -> Image

Indicates whether SwiftUI renders an image as-is, or by using a different mode.

func interpolation(Image.Interpolation) -> Image

Specifies the current level of quality for rendering an image that requires interpolation.

enum TemplateRenderingMode

A type that indicates how SwiftUI renders images.

enum Interpolation

The level of quality for rendering an image that requires interpolation, such as a scaled image.

