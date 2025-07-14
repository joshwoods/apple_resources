

- SwiftUI
- GraphicsContext
- GraphicsContext.Filter
-  colorMultiply(\_:) 

Type Method

# colorMultiply(\_:)

Returns a filter that multiplies each color component by the matching component of a given color.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func colorMultiply(_ color: Color) -> GraphicsContext.Filter
```

## Parameters 

`color`  

The color that the filter uses for the multiplication operation.

## Return Value

A filter that multiplies color components.

## See Also

### Manipulating color

static func saturation(Double) -> GraphicsContext.Filter

Returns a filter that applies a saturation adjustment.

static func colorInvert(Double) -> GraphicsContext.Filter

Returns a filter that inverts the color of their results.

static func hueRotation(Angle) -> GraphicsContext.Filter

Returns a filter that applies a hue rotation adjustment.

static func grayscale(Double) -> GraphicsContext.Filter

Returns a filter that applies a grayscale adjustment.

static func colorMatrix(ColorMatrix) -> GraphicsContext.Filter

Returns a filter that multiplies by a given color matrix.

