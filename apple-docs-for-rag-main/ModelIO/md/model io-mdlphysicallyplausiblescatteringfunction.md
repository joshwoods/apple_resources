

- Model I/O
-  MDLPhysicallyPlausibleScatteringFunction 

Class

# MDLPhysicallyPlausibleScatteringFunction

A set of material properties that describes a physically realistic shading model for materials.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class MDLPhysicallyPlausibleScatteringFunction
```

## Overview

The set of material properties that define a material’s response to lighting is also called the *Bidirectional Reflectance Distribution Function*, or BRDF, for surfaces shaded using that MDLMaterial object. The properties defined by this class, along with some properties inherited from the superclass MDLScatteringFunction, describe a shading model that more closely simulates real-world lighting physics than traditional shading models. (This shading model is similar to those used in recent game engines and feature films.)

The valid range for each material property in this shading function is `0.0` to `1.0`, inclusive. Creating a new scattering function object with the inherited init() method creates a set of material properties with useful default values for this shading model.

## Topics

### Working with Shading Properties

var subsurface: MDLMaterialProperty

The degree to which light scatters under the surface of the material.

var metallic: MDLMaterialProperty

The degree to which the material appears as a dielectric surface (lower values) or as a metal (higher values).

var specularAmount: MDLMaterialProperty

The tendency of the material to generate specular highlights.

var specularTint: MDLMaterialProperty

The balance of color for specular highlights, between the light color (lower values) and the material’s base color (at higher values).

var roughness: MDLMaterialProperty

The degree to which a material appears smooth, affecting both diffuse and specular response.

var anisotropic: MDLMaterialProperty

The degree to which specular highlights elongate in the direction of the local tangent basis.

var anisotropicRotation: MDLMaterialProperty

The angle at which anisotropic effects are rotated relative to the local tangent basis.

var sheen: MDLMaterialProperty

The intensity of highlights that appear only at glancing angles on a material’s surface.

var sheenTint: MDLMaterialProperty

The balance of color for highlights that appear only at glancing angles, between the light color (lower values) and the material’s base color (at higher values).

var clearcoat: MDLMaterialProperty

The intensity of a second specular highlight, similar to the gloss that results from a clear coat on an automotive finish.

var clearcoatGloss: MDLMaterialProperty

The sharpness of a second specular highlight, similar to the gloss that results from a clear coat on an automotive finish.

### Instance Properties

var version: Int

## Relationships

### Inherits From

- MDLScatteringFunction

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

class MDLScatteringFunction

A set of material properties that describes a basic shading model for materials, and the superclass for more complex shading models.

