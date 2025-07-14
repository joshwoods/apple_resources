

- Model I/O
-  MDLScatteringFunction 

Class

# MDLScatteringFunction

A set of material properties that describes a basic shading model for materials, and the superclass for more complex shading models.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class MDLScatteringFunction
```

## Overview

The set of material properties that define a material’s response to lighting is also called the *Bidirectional Reflectance Distribution Function*, or BRDF, for surfaces shaded using that MDLMaterial object. The set of properties defined by the MDLScatteringFunction class itself describes a Lambertian shading model with Blinn-Phong specular response; subclasses can define a set of properties for other shading models.

Creating a new scattering function object with the inherited init() method creates a set of material properties with useful default values for this shading model.

## Topics

### Naming a Scattering Function

var name: String

A descriptive name for the scattering function.

### Working with Shading Properties

var baseColor: MDLMaterialProperty

The inherent color of the material, to be used as a modulator during shading.

var emission: MDLMaterialProperty

The color emitted as radiance from a material’s surface.

var specular: MDLMaterialProperty

The intensity of specular highlights on the material’s surface.

var materialIndexOfRefraction: MDLMaterialProperty

The index of refraction for the medium surrounding a material.

var interfaceIndexOfRefraction: MDLMaterialProperty

The index of refraction for a material itself.

var normal: MDLMaterialProperty

The variation in the surface normal vectors in a material, relative to model coordinate space.

var ambientOcclusion: MDLMaterialProperty

The attenuation of ambient light due to local geometry variations on a surface.

var ambientOcclusionScale: MDLMaterialProperty

The scaling factor for ambient occlusion shading.

## Relationships

### Inherits From

- NSObject

### Inherited By

- MDLPhysicallyPlausibleScatteringFunction

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MDLNamed
- NSObjectProtocol

## See Also

### Materials

class MDLMaterial

A collection of material properties that together describe the intended surface appearance for rendering a 3D object.

class MDLMaterialProperty

A definition for one specific aspect of the rendering parameters for a material.

class MDLMaterialPropertyConnection

class MDLMaterialPropertyGraph

class MDLMaterialPropertyNode

class MDLPhysicallyPlausibleScatteringFunction

A set of material properties that describes a physically realistic shading model for materials.

