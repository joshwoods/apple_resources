

- Model I/O
-  MDLLightProbe 

Class

# MDLLightProbe

A light source described in terms of the variations in color and intensity of its illumination in all directions.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class MDLLightProbe
```

## Overview

A light probe represents this variation either as a cube map texture or as a set of spherical harmonic coefficients. In addition to describing such light sources, the MDLLightProbe class provides methods for generating light probe textures based on the contents of a scene and for generating spherical harmonic coefficients from a texture.

A light probe consists of two cube map textures, where each texel represents the color and intensity of light in a particular direction from the cube’s center:

- The reflectiveTexture cube map, also known as an *environment map*, contains a rendering of a scene as viewed from the light probe’s position. A renderer can use this texture to create reflections on surfaces with metallic materials.

- The irradianceTexture cube map contains samples of the total light arriving at the light probe’s position from every direction. A renderer can use this texture to create diffuse lighting effects. You can derive an irradiance map from an environment map with methods on the MDLTexture class, or when creating a light probe with the init(textureSize:forLocation:lightsToConsider:objectsToConsider:reflectiveCubemap:irradianceCubemap:) method.

Using cube map textures for light-probe-based rendering offers great visual fidelity, but adversely affects performance due to the cost of texture lookups during rendering. In addition, a cube map texture often contains more detail than is necessary for lighting. A set of spherical harmonic coefficients can represent the same information with less detail, and can be used in shader calculations with much less performance cost. To use spherical harmonics, call the generateSphericalHarmonics(fromIrradiance:) method, then access the generated data in the sphericalHarmonicsCoefficients property.

## Topics

### Creating a Light Probe

init(reflectiveTexture: MDLTexture?, irradianceTexture: MDLTexture?)

Initializes a light probe with the specified cube map textures.

### Working with Textures

var reflectiveTexture: MDLTexture?

A cube map texture that contains a rendering of a scene as seen from the light probe’s position.

var irradianceTexture: MDLTexture?

A cube map texture that contains samples of the total light arriving at the light probe’s position from every direction.

### Working with Spherical Harmonics

func generateSphericalHarmonics(fromIrradiance: Int)

Generates spherical harmonics information based on the light probe’s irradiance texture.

var sphericalHarmonicsCoefficients: Data?

Data containing the spherical harmonics coefficients for the light.

var sphericalHarmonicsLevel: Int

The number of levels of spherical harmonics information in the light probe.

### Generating Light Probes from Scene Contents

init?(textureSize: Int, forLocation: MDLTransform, lightsToConsider: [MDLLight], objectsToConsider: [MDLObject], reflectiveCubemap: MDLTexture?, irradianceCubemap: MDLTexture?)

Creates a light probe representing the shading environment at a specific point in a scene.

## Relationships

### Inherits From

- MDLLight

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

protocol MDLLightProbeIrradianceDataSource

Adopt this protocol to provide information for use in automatic placement of light probes around a scene.

class MDLPhotometricLight

A light source whose shape, direction, and intensity of illumination are determined by a photometric profile.

class MDLPhysicallyPlausibleLight

A light source for use in shading models based on real-world physics.

