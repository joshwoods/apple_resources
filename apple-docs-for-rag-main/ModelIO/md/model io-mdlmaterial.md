

- Model I/O
-  MDLMaterial 

Class

# MDLMaterial

A collection of material properties that together describe the intended surface appearance for rendering a 3D object.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class MDLMaterial
```

## Overview

Each material property (a MDLMaterialProperty object) provides one specific aspect of appearance, such as opacity, shininess, or surface detail. Use the material property of a MDLSubmesh object to associate a material with a 3D object for rendering or to find the material assigned to an object loaded from an asset file.

Sets of certain material properties called *scattering functions* determine the material’s response to lighting. You can manage these properties together using a material’s scatteringFunction property. Creating a material with the inherited init() initializer is equivalent to using the init(name:scatteringFunction:) with a MDLScatteringFunction object whose properties all have default values.

## Topics

### Creating a material

init(name: String, scatteringFunction: MDLScatteringFunction)

Initializes a material

### Using a material

var materialFace: MDLMaterialFace

The surface of an object.

var name: String

A descriptive name for the material.

### Determining a material’s response to lighting

var scatteringFunction: MDLScatteringFunction

The collection of material properties that define the material’s response to light.

### Working with individual material properties

func propertyNamed(String) -> MDLMaterialProperty?

Returns the material property with the specified name.

func property(with: MDLMaterialSemantic) -> MDLMaterialProperty?

Returns the material property for the specified material semantic.

func properties(with: MDLMaterialSemantic) -> [MDLMaterialProperty]

Returns the complete list of material properties that match the specified material semantic.

func setProperty(MDLMaterialProperty)

Adds a new material property to or replaces an existing material property in the material.

func remove(MDLMaterialProperty)

Removes the specified material property from the material.

func removeAllProperties()

Removes all material properties from the material.

### Sharing material properties

var base: MDLMaterial?

Another material object from which this material’s properties are derived.

### Accessing material properties with subscript syntax

subscript(String) -> MDLMaterialProperty?

Returns the material property with the specified name, for use with subscript syntax.

subscript(Int) -> MDLMaterialProperty?

Returns the material property at the specified index in the material, for use with subscript syntax.

var count: Int

The number of material properties in the material.

### Working with textures using resolvers

func loadTextures(using: any MDLAssetResolver)

Loads textures using resolver for string paths and NSURLs.

func resolveTextures(with: any MDLAssetResolver)

Resolves all texture string paths as NSURLs with resolver.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MDLNamed
- NSFastEnumeration
- NSObjectProtocol

## See Also

### Materials

class MDLMaterialProperty

A definition for one specific aspect of the rendering parameters for a material.

class MDLMaterialPropertyConnection

class MDLMaterialPropertyGraph

class MDLMaterialPropertyNode

class MDLScatteringFunction

A set of material properties that describes a basic shading model for materials, and the superclass for more complex shading models.

class MDLPhysicallyPlausibleScatteringFunction

A set of material properties that describes a physically realistic shading model for materials.

