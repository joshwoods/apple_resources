

- Metal
-  MTLBlendOperation 

Enumeration

# MTLBlendOperation

For every pixel, `MTLBlendOperation` determines how to combine and weight the source fragment values with the destination values. Some blend operations multiply the source values by a source blend factor (SBF), multiply the destination values by a destination blend factor (DBF), and then combine the results using addition or subtraction. Other blend operations use either a minimum or maximum function to determine the result.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
enum MTLBlendOperation
```

## Topics

### Constants

case add

Add portions of both source and destination pixel values.

case subtract

Subtract a portion of the destination pixel values from a portion of the source.

case reverseSubtract

Subtract a portion of the source values from a portion of the destination pixel values.

case min

Minimum of the source and destination pixel values.

case max

Maximum of the source and destination pixel values.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum MTLBlendFactor

The source and destination blend factors are often needed to complete specification of a blend operation. In most cases, the blend factor for both RGB values (*F(rgb)*) and alpha values (*F(a)*) are similar to one another, but in some cases, such as `MTLBlendFactorSourceAlphaSaturated`, the blend factor is slightly different. Four blend factors (`MTLBlendFactorBlendColor`, `MTLBlendFactorOneMinusBlendColor`, `MTLBlendFactorBlendAlpha`, and `MTLBlendFactorOneMinusBlendAlpha`) refer to a constant blend color value that is set by the setBlendColor(red:green:blue:alpha:) method of `MTLRenderCommandEncoder`.

struct MTLColorWriteMask

Values used to specify a mask to permit or restrict writing to color channels of a color value. The values red, green, blue, and alpha select one color channel each, and they can be bitwise combined.

