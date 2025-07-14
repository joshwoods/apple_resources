

- Core Graphics
-  CGGradientDrawingOptions 

Structure

# CGGradientDrawingOptions

Drawing locations for gradients.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CGGradientDrawingOptions
```

## Topics

### Constants

static var drawsBeforeStartLocation: CGGradientDrawingOptions

The fill should extend beyond the starting location. The color that extends beyond the starting point is the solid color defined by the CGGradient object to be at location 0.

static var drawsAfterEndLocation: CGGradientDrawingOptions

The fill should extend beyond the ending location. The color that extends beyond the ending point is the solid color defined by the CGGradient object to be at location 1.

### Initializers

init(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Drawing Gradients and Shadings

func drawLinearGradient(CGGradient, start: CGPoint, end: CGPoint, options: CGGradientDrawingOptions)

Paints a gradient fill that varies along the line defined by the provided starting and ending points.

func drawRadialGradient(CGGradient, startCenter: CGPoint, startRadius: CGFloat, endCenter: CGPoint, endRadius: CGFloat, options: CGGradientDrawingOptions)

Paints a gradient fill that varies along the area defined by the provided starting and ending circles.

func drawShading(CGShading)

Fills the clipping path of a context with the specified shading.

