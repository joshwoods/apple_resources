

- SwiftUI
- GraphicsContext
- GraphicsContext.Filter
-  hueRotation(\_:) 

Type Method

# hueRotation(\_:)

Returns a filter that applies a hue rotation adjustment.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func hueRotation(_ angle: Angle) -> GraphicsContext.Filter
```

## Parameters 

`angle`  

The amount by which to rotate the hue value of each pixel.

## Return Value

A filter that applies a hue rotation adjustment.

## Discussion

This filter is equivalent to the `hue-rotate` filter primitive defined by the Scalable Vector Graphics (SVG) specification.

## See Also

### Manipulating color

static func saturation(Double) -> GraphicsContext.Filter

Returns a filter that applies a saturation adjustment.

static func colorInvert(Double) -> GraphicsContext.Filter

Returns a filter that inverts the color of their results.

static func colorMultiply(Color) -> GraphicsContext.Filter

Returns a filter that multiplies each color component by the matching component of a given color.

static func grayscale(Double) -> GraphicsContext.Filter

Returns a filter that applies a grayscale adjustment.

static func colorMatrix(ColorMatrix) -> GraphicsContext.Filter

Returns a filter that multiplies by a given color matrix.

