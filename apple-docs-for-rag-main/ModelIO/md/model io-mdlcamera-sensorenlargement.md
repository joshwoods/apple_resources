

- Model I/O
- MDLCamera
-  sensorEnlargement 

Instance Property

# sensorEnlargement

The horizontal and vertical scale factors that determine the active region of the sensor.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var sensorEnlargement: vector_float2 { get set }
```

## Discussion

For example, an enlargement factor of `{2,2}` results in the center portion of the image being cropped and expanded to fill the image plane. The default factor is `1.0` in both directions.

## See Also

### Modeling a Physical Imaging Surface

var sensorVerticalAperture: Float

The height, in millimeters, of the camera’s simulated imaging surface.

var sensorAspect: Float

The ratio of width to height for the camera’s simulated imaging surface.

var sensorShift: vector_float2

The horizontal and vertical offsets, in millimeters, of the center of the camera image relative to the center of the simulated lens.

var flash: vector_float3

Red, green, and blue factors to be used in brightening darker areas of the camera’s image.

var exposure: vector_float3

Red, green, and blue factors that scale each color channel in the camera’s image.

var exposureCompression: vector_float2

Two parameters that determine the brightness compression curve for colors in the camera’s image.

