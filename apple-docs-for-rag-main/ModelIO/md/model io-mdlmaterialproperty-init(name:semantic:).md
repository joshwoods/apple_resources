

- Model I/O
- MDLMaterialProperty
-  init(name:semantic:) 

Initializer

# init(name:semantic:)

Initializes a material property without a value.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(
    name: String,
    semantic: MDLMaterialSemantic
)
```

## Parameters 

`name`  

A descriptive name for the material property. For details, see the name property.

`semantic`  

The semantic meaning for the material property’s value. For details, see the semantic property.

## Return Value

A new material property object.

## Discussion

The newly created material property’s value is empty, and its type property is MDLMaterialPropertyType.none. Use one of the properties listed in Working with a Material Property’s Value to provide a value for the material property.

## See Also

### Creating a Material Property

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

