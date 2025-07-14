

- SwiftUI
- Image
-  antialiased(\_:) 

Instance Method

# antialiased(\_:)

Specifies whether SwiftUI applies antialiasing when rendering the image.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func antialiased(_ isAntialiased: Bool) -> Image
```

## Parameters 

`isAntialiased`  

A Boolean value that specifies whether to allow antialiasing. Pass `true` to allow antialising, `false` otherwise.

## Return Value

An image with the antialiasing behavior set.

## See Also

### Specifying rendering behavior

func symbolRenderingMode(SymbolRenderingMode?) -> Image

Sets the rendering mode for symbol images within this view.

func renderingMode(Image.TemplateRenderingMode?) -> Image

Indicates whether SwiftUI renders an image as-is, or by using a different mode.

func interpolation(Image.Interpolation) -> Image

Specifies the current level of quality for rendering an image that requires interpolation.

enum TemplateRenderingMode

A type that indicates how SwiftUI renders images.

enum Interpolation

The level of quality for rendering an image that requires interpolation, such as a scaled image.

