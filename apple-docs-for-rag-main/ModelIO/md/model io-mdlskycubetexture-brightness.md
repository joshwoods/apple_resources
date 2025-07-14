

- Model I/O
- MDLSkyCubeTexture
-  brightness 

Instance Property

# brightness

The amount of brightness enhancement to apply during tone mapping.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var brightness: Float { get set }
```

## Discussion

To render a sky texture, Model I/O first simulates the colors visible in the sky at different directions and then applies tone mapping to fit the resulting colors into the range of displayable values. As part of this process, Model I/O uses this property to scale the brightness of the texture image.

## See Also

### Working with Tone Mapping Parameters

var gamma: Float

The amount of gamma correction to apply during tone mapping.

var exposure: Float

The amount of exposure compensation to apply during tone mapping.

var contrast: Float

The amount of contrast enhancement to apply during tone mapping.

var saturation: Float

The amount of saturation enhancement to apply during tone mapping.

var highDynamicRangeCompression: vector_float2

Two parameters that determine the brightness compression curve for colors in the texture image.

