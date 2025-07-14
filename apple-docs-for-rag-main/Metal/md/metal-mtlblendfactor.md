

- Metal
-  MTLBlendFactor 

Enumeration

# MTLBlendFactor

The source and destination blend factors are often needed to complete specification of a blend operation. In most cases, the blend factor for both RGB values (*F(rgb)*) and alpha values (*F(a)*) are similar to one another, but in some cases, such as `MTLBlendFactorSourceAlphaSaturated`, the blend factor is slightly different. Four blend factors (`MTLBlendFactorBlendColor`, `MTLBlendFactorOneMinusBlendColor`, `MTLBlendFactorBlendAlpha`, and `MTLBlendFactorOneMinusBlendAlpha`) refer to a constant blend color value that is set by the setBlendColor(red:green:blue:alpha:) method of `MTLRenderCommandEncoder`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
enum MTLBlendFactor
```

## Topics

### Constants

case zero

Blend factor of zero.

case one

Blend factor of one.

case sourceColor

Blend factor of source values.

case oneMinusSourceColor

Blend factor of one minus source values.

case sourceAlpha

Blend factor of source alpha.

case oneMinusSourceAlpha

Blend factor of one minus source alpha.

case destinationColor

Blend factor of destination values.

case oneMinusDestinationColor

Blend factor of one minus destination values.

case destinationAlpha

Blend factor of destination alpha.

case oneMinusDestinationAlpha

Blend factor of one minus destination alpha.

case sourceAlphaSaturated

Blend factor of the minimum of either source alpha or one minus destination alpha.

case blendColor

Blend factor of RGB values.

case oneMinusBlendColor

Blend factor of one minus RGB values.

case blendAlpha

Blend factor of alpha value.

case oneMinusBlendAlpha

Blend factor of one minus alpha value.

case source1Color

Blend factor of source values. This option supports dual-source blending and reads from the second color output of the fragment function.

case oneMinusSource1Color

Blend factor of one minus source values. This option supports dual-source blending and reads from the second color output of the fragment function.

case source1Alpha

Blend factor of source alpha. This option supports dual-source blending and reads from the second color output of the fragment function.

case oneMinusSource1Alpha

Blend factor of one minus source alpha. This option supports dual-source blending and reads from the second color output of the fragment function.

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

enum MTLBlendOperation

For every pixel, `MTLBlendOperation` determines how to combine and weight the source fragment values with the destination values. Some blend operations multiply the source values by a source blend factor (SBF), multiply the destination values by a destination blend factor (DBF), and then combine the results using addition or subtraction. Other blend operations use either a minimum or maximum function to determine the result.

struct MTLColorWriteMask

Values used to specify a mask to permit or restrict writing to color channels of a color value. The values red, green, blue, and alpha select one color channel each, and they can be bitwise combined.

