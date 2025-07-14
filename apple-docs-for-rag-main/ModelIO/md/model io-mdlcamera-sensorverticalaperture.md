

- Model I/O
- MDLCamera
-  sensorVerticalAperture 

Instance Property

# sensorVerticalAperture

The height, in millimeters, of the camera’s simulated imaging surface.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var sensorVerticalAperture: Float { get set }
```

## Discussion

In a physically based camera, field of view is based on the focal length of the lens and the vertical aperture of the imaging surface (film or sensor). Changing the focalLength or sensorVerticalAperture property updates the fieldOfView property to the corresponding value, and vice versa.

To determine the width of the imaging surface, use this property and the sensorAspect property. For example, with the default vertical aperture of 24mm and default aspect ratio of 1.5 (or 3:2), the horizontal aperture is 36mm.

## See Also

### Modeling a Physical Imaging Surface

var sensorAspect: Float

The ratio of width to height for the camera’s simulated imaging surface.

var sensorEnlargement: vector_float2

The horizontal and vertical scale factors that determine the active region of the sensor.

var sensorShift: vector_float2

The horizontal and vertical offsets, in millimeters, of the center of the camera image relative to the center of the simulated lens.

var flash: vector_float3

Red, green, and blue factors to be used in brightening darker areas of the camera’s image.

var exposure: vector_float3

Red, green, and blue factors that scale each color channel in the camera’s image.

var exposureCompression: vector_float2

Two parameters that determine the brightness compression curve for colors in the camera’s image.

