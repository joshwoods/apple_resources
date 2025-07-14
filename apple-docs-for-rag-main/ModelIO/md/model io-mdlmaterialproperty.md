

- Model I/O
-  MDLMaterialProperty 

Class

# MDLMaterialProperty

A definition for one specific aspect of the rendering parameters for a material.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class MDLMaterialProperty
```

## Overview

The collection of material properties in a MDLMaterial instance defines the intended surface appearance for rendering a 3D object. A material property object’s semantic property identifies which aspect of material rendering it affects, and its value (which can be any of several types) determines how the material property contributes to that aspect of rendering.

When you initialize a material property with a specific value (using one of the initializers listed in Creating a Material Property) or set the value of an existing material property (using one of the property setters listed in Working with a Material Property’s Value), the type property changes to reflect the data type of the stored value. To retrieve the material property’s value, you must use the property accessor appropriate to its type. If you read a material property’s value using an accessor for a different type, the result is undefined.

## Topics

### Creating a Material Property

init(name: String, semantic: MDLMaterialSemantic)

Initializes a material property without a value.

convenience init(name: String, semantic: MDLMaterialSemantic, string: String?)

Initializes a material property with a string value.

convenience init(name: String, semantic: MDLMaterialSemantic, url: URL?)

Initializes a material property with a URL value.

convenience init(name: String, semantic: MDLMaterialSemantic, textureSampler: MDLTextureSampler?)

Initializes a material property with a texture sampler object.

convenience init(name: String, semantic: MDLMaterialSemantic, color: CGColor)

Initializes a material property with a color value.

convenience init(name: String, semantic: MDLMaterialSemantic, float: Float)

Initializes a material property with a scalar value.

convenience init(name: String, semantic: MDLMaterialSemantic, float2: vector_float2)

Initializes a material property with a 2-component vector value.

convenience init(name: String, semantic: MDLMaterialSemantic, float3: vector_float3)

Initializes a material property with a 3-component vector value.

convenience init(name: String, semantic: MDLMaterialSemantic, float4: vector_float4)

Initializes a material property with a 4-component vector value.

convenience init(name: String, semantic: MDLMaterialSemantic, matrix4x4: matrix_float4x4)

Initializes a material property with a 4 x 4 matrix value.

### Using a Material Property

var name: String

A descriptive name for the material property.

var semantic: MDLMaterialSemantic

The semantic meaning for the material property’s value.

var type: MDLMaterialPropertyType

The data type stored in the material property’s value.

### Working with a Material Property’s Value

var stringValue: String?

The string value for the material.

var urlValue: URL?

The URL value for the material property—typically, the URL to a texture image.

var textureSamplerValue: MDLTextureSampler?

A texture sampler object that provides the texture image value for the material property.

var color: CGColor?

The color value for the material property.

var floatValue: Float

The scalar floating-point value for the material property.

var float2Value: vector_float2

The 2-component floating-point vector value for the material property.

var float3Value: vector_float3

The 3-component floating-point vector value for the material property.

var float4Value: vector_float4

The 4-component floating-point vector value for the material property.

var matrix4x4: matrix_float4x4

The 4 x 4 floating-point matrix value for the material property.

### Copying a Material Property

func setProperties(MDLMaterialProperty)

Sets the material property’s attributes to those of the specified material property.

### Constants

enum MDLMaterialSemantic

Options for the semantic use of a material property’s value in rendering a particular surface appearance; used by the semantic property.

enum MDLMaterialPropertyType

Options for the data type of a material property, used by the type property.

### Instance Properties

var luminance: Float

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
- NSCopying
- NSObjectProtocol

## See Also

### Materials

class MDLMaterial

A collection of material properties that together describe the intended surface appearance for rendering a 3D object.

class MDLMaterialPropertyConnection

class MDLMaterialPropertyGraph

class MDLMaterialPropertyNode

class MDLScatteringFunction

A set of material properties that describes a basic shading model for materials, and the superclass for more complex shading models.

class MDLPhysicallyPlausibleScatteringFunction

A set of material properties that describes a physically realistic shading model for materials.

