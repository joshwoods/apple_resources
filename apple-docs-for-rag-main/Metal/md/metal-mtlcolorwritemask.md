

- Metal
-  MTLColorWriteMask 

Structure

# MTLColorWriteMask

Values used to specify a mask to permit or restrict writing to color channels of a color value. The values red, green, blue, and alpha select one color channel each, and they can be bitwise combined.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
struct MTLColorWriteMask
```

## Topics

### Initializers

init(rawValue: UInt)

Returns a new color write mask from a specified raw value.

### Constants

static var red: MTLColorWriteMask

The red color channel is enabled.

static var green: MTLColorWriteMask

The green color channel is enabled.

static var blue: MTLColorWriteMask

The blue color channel is enabled.

static var alpha: MTLColorWriteMask

The alpha color channel is enabled.

static var all: MTLColorWriteMask

All color channels are enabled.

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

### Constants

enum MTLBlendOperation

For every pixel, `MTLBlendOperation` determines how to combine and weight the source fragment values with the destination values. Some blend operations multiply the source values by a source blend factor (SBF), multiply the destination values by a destination blend factor (DBF), and then combine the results using addition or subtraction. Other blend operations use either a minimum or maximum function to determine the result.

enum MTLBlendFactor

The source and destination blend factors are often needed to complete specification of a blend operation. In most cases, the blend factor for both RGB values (*F(rgb)*) and alpha values (*F(a)*) are similar to one another, but in some cases, such as `MTLBlendFactorSourceAlphaSaturated`, the blend factor is slightly different. Four blend factors (`MTLBlendFactorBlendColor`, `MTLBlendFactorOneMinusBlendColor`, `MTLBlendFactorBlendAlpha`, and `MTLBlendFactorOneMinusBlendAlpha`) refer to a constant blend color value that is set by the setBlendColor(red:green:blue:alpha:) method of `MTLRenderCommandEncoder`.

