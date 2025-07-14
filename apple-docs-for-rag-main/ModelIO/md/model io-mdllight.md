

- Model I/O
-  MDLLight 

Class

# MDLLight

The abstract superclass for objects that describe light sources in a scene.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class MDLLight
```

## Overview

When you load lights from an asset file using the MDLAsset class or create lights when building an asset for export, you use one or more of the concrete subclasses MDLPhysicallyPlausibleLight, MDLAreaLight, MDLPhotometricLight, or MDLLightProbe.

## Topics

### Working with Lights

func irradiance(atPoint: vector_float3) -> Unmanaged&lt;CGColor>

Returns the radiance of the light as received at a specific point in the same scene.

func irradiance(atPoint: vector_float3, colorSpace: CGColorSpace) -> Unmanaged&lt;CGColor>

Returns the radiance of the light as received at a specific point in the same scene, expressed using the specified color space.

var lightType: MDLLightType

The type of the light.

var colorSpace: String

The name of the Core Graphics color space to be used for interpreting the light’s color information.

### Constants

enum MDLLightType

Options for the shape and style of illumination provided by a light, used by the lightType property.

## Relationships

### Inherits From

- MDLObject

### Inherited By

- MDLLightProbe
- MDLPhysicallyPlausibleLight

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

class MDLAreaLight

A light source that illuminates a 3D scene from an area with a specific shape.

class MDLLightProbe

A light source described in terms of the variations in color and intensity of its illumination in all directions.

protocol MDLLightProbeIrradianceDataSource

Adopt this protocol to provide information for use in automatic placement of light probes around a scene.

class MDLPhotometricLight

A light source whose shape, direction, and intensity of illumination are determined by a photometric profile.

class MDLPhysicallyPlausibleLight

A light source for use in shading models based on real-world physics.

