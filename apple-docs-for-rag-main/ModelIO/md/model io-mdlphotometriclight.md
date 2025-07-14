

- Model I/O
-  MDLPhotometricLight 

Class

# MDLPhotometricLight

A light source whose shape, direction, and intensity of illumination are determined by a photometric profile.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class MDLPhotometricLight
```

## Overview

You create a photometric light from a file in the IES format, containing physical measurements of a light source. Many manufacturers of real-world light fixtures publish such files describing the lighting characteristics of their products. This photometry data measures the light web surrounding a light source—measurements of the light’s intensity in all directions around the source.The MDLPhotometricLight provides two ways to interpret a light web:

- As a cube map texture. Use the generateCubemap(fromLight:) method to generate a texture, then use the lightCubeMap property to access the texture. In this texture, each texel represents the light’s intensity in the direction from the cube’s center to the texel’s position on the cube.

- **As spherical harmonics.** Use the generateSphericalHarmonics(fromLight:) method to generate a set of spherical harmonic coefficients, and then use the sphericalHarmonicsLevel and sphericalHarmonicsCoefficients properties to access these coefficients. Spherical harmonic coefficients provide a more compact representation of the same information as the cube map texture, so you can use them during shading without the performance cost of a texture lookup.

Both the MDLPhotometricLight and MDLAreaLight classes can describe lights with interesting shapes—an area light offers a simpler design that can be implemented with better rendering performance, and a photometric light offers design that better models real-world light fixtures at the cost of higher computational complexity.

## Topics

### Creating a Photometric Light

init?(iesProfile: URL)

Initializes a light from photometry data in the file at the specified URL.

### Interpreting the Light Web as a Cube Texture

func generateCubemap(fromLight: Int)

Generates a cube map texture from the light’s photometry data.

var lightCubeMap: MDLTexture?

A cube map texture describing the light’s intensity in all directions.

### Interpreting the Light Web as Spherical Harmonics

func generateSphericalHarmonics(fromLight: Int)

Generates spherical harmonics information based on the light’s photometry data.

var sphericalHarmonicsCoefficients: Data?

Data containing spherical harmonics coefficients that describe the light’s intensity in all directions.

var sphericalHarmonicsLevel: Int

The number of levels of generated spherical harmonics information.

### Instance Methods

func generateTexture(Int) -> MDLTexture

## Relationships

### Inherits From

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

class MDLLight

The abstract superclass for objects that describe light sources in a scene.

class MDLAreaLight

A light source that illuminates a 3D scene from an area with a specific shape.

class MDLLightProbe

A light source described in terms of the variations in color and intensity of its illumination in all directions.

protocol MDLLightProbeIrradianceDataSource

Adopt this protocol to provide information for use in automatic placement of light probes around a scene.

class MDLPhysicallyPlausibleLight

A light source for use in shading models based on real-world physics.

