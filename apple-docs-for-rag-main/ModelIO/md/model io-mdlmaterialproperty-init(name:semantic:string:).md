

- Model I/O
- MDLMaterialProperty
-  init(name:semantic:string:) 

Initializer

# init(name:semantic:string:)

Initializes a material property with a string value.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
convenience init(
    name: String,
    semantic: MDLMaterialSemantic,
    string: String?
)
```

## Parameters 

`name`  

A descriptive name for the material property. For details, see the name property.

`semantic`  

The semantic meaning for the material property’s value. For details, see the semantic property.

`string`  

The string value for the material.

## Return Value

A new material property object whose type property is MDLMaterialPropertyType.string.

## Discussion

The meaning of a string value depends on the renderer (or other software component) processing the material. For example, a string value might be treated as the name of a texture image to be loaded from a default path.

## See Also

### Creating a Material Property

init(name: String, semantic: MDLMaterialSemantic)

Initializes a material property without a value.

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

