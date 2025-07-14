

- Model I/O
-  MDLPhysicallyPlausibleLight 

Class

# MDLPhysicallyPlausibleLight

A light source for use in shading models based on real-world physics.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class MDLPhysicallyPlausibleLight
```

## Topics

### Managing Light Color and Intensity

var color: CGColor?

The color of the light source.

var lumens: Float

The total visible intensity of the light source, in lumens.

func setColorByTemperature(Float)

Sets the light’s color based on a black-body temperature.

### Managing Light Geometry

var innerConeAngle: Float

The radial angle, in degrees, of the area fully illuminated by the light.

var outerConeAngle: Float

The radial angle, in degrees, at which the illumination from a spotlight becomes zero.

### Managing Attenuation

var attenuationStartDistance: Float

The distance from the light source, in units of local coordinate space, at which its illumination begins to diminish.

var attenuationEndDistance: Float

The distance from the light source, in units of local coordinate space, at which its illumination becomes zero.

## Relationships

### Inherits From

- MDLLight

### Inherited By

- MDLAreaLight
- MDLPhotometricLight

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MDLNamed
- NSObjectProtocol

## See Also

### Lights

class MDLLight

The abstract superclass for objects that describe light sources in a scene.

class MDLAreaLight

A light source that illuminates a 3D scene from an area with a specific shape.

class MDLLightProbe

A light source described in terms of the variations in color and intensity of its illumination in all directions.

protocol MDLLightProbeIrradianceDataSource

Adopt this protocol to provide information for use in automatic placement of light probes around a scene.

class MDLPhotometricLight

A light source whose shape, direction, and intensity of illumination are determined by a photometric profile.

