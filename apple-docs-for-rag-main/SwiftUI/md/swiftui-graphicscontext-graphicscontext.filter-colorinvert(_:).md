

- SwiftUI
- GraphicsContext
- GraphicsContext.Filter
-  colorInvert(\_:) 

Type Method

# colorInvert(\_:)

Returns a filter that inverts the color of their results.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func colorInvert(_ amount: Double = 1) -> GraphicsContext.Filter
```

## Parameters 

`amount`  

The inversion amount. A value of one results in total inversion, while a value of zero leaves the result unchanged. Other values apply a linear multiplier effect.

## Return Value

A filter that applies a color inversion.

## Discussion

This filter is equivalent to the `invert` filter primitive defined by the Scalable Vector Graphics (SVG) specification.

## See Also

### Manipulating color

static func saturation(Double) -> GraphicsContext.Filter

Returns a filter that applies a saturation adjustment.

static func colorMultiply(Color) -> GraphicsContext.Filter

Returns a filter that multiplies each color component by the matching component of a given color.

static func hueRotation(Angle) -> GraphicsContext.Filter

Returns a filter that applies a hue rotation adjustment.

static func grayscale(Double) -> GraphicsContext.Filter

Returns a filter that applies a grayscale adjustment.

static func colorMatrix(ColorMatrix) -> GraphicsContext.Filter

Returns a filter that multiplies by a given color matrix.

