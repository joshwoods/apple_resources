

- SwiftUI
- Image
-  interpolation(\_:) 

Instance Method

# interpolation(\_:)

Specifies the current level of quality for rendering an image that requires interpolation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func interpolation(_ interpolation: Image.Interpolation) -> Image
```

## Parameters 

`interpolation`  

The quality level, expressed as a value of the `Interpolation` type, that SwiftUI applies when interpolating an image.

## Return Value

An image with the given interpolation value set.

## Mentioned in 

Fitting images into available space

## Discussion

See the article Fitting images into available space for examples of using `interpolation(_:)` when scaling an Image.

## See Also

### Specifying rendering behavior

func antialiased(Bool) -> Image

Specifies whether SwiftUI applies antialiasing when rendering the image.

func symbolRenderingMode(SymbolRenderingMode?) -> Image

Sets the rendering mode for symbol images within this view.

func renderingMode(Image.TemplateRenderingMode?) -> Image

Indicates whether SwiftUI renders an image as-is, or by using a different mode.

enum TemplateRenderingMode

A type that indicates how SwiftUI renders images.

enum Interpolation

The level of quality for rendering an image that requires interpolation, such as a scaled image.

