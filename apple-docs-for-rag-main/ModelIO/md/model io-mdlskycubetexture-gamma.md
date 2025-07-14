

- Model I/O
- MDLSkyCubeTexture
-  gamma 

Instance Property

# gamma

The amount of gamma correction to apply during tone mapping.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var gamma: Float { get set }
```

## Discussion

To render a sky texture, Model I/O first simulates the colors visible in the sky at different directions and then applies tone mapping to fit the resulting colors into the range of displayable values. As part of this process, Model I/O applies this property to the gamma curve of the texture image.

## See Also

### Working with Tone Mapping Parameters

var exposure: Float

The amount of exposure compensation to apply during tone mapping.

var brightness: Float

The amount of brightness enhancement to apply during tone mapping.

var contrast: Float

The amount of contrast enhancement to apply during tone mapping.

var saturation: Float

The amount of saturation enhancement to apply during tone mapping.

var highDynamicRangeCompression: vector_float2

Two parameters that determine the brightness compression curve for colors in the texture image.

