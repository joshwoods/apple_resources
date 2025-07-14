

- Metal
- MTLBlendFactor
-  MTLBlendFactor.sourceColor 

Case

# MTLBlendFactor.sourceColor

Blend factor of source values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
case sourceColor
```

## Discussion

`F(rgb) = Source.rgb`

`F(a) = Source.a`

## See Also

### Constants

case zero

Blend factor of zero.

case one

Blend factor of one.

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

