

- Model I/O
- MDLMaterialProperty
-  floatValue 

Instance Property

# floatValue

The scalar floating-point value for the material property.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var floatValue: Float { get set }
```

## Discussion

Scalar values are appropriate for some semantics, such as the MDLMaterialSemantic.specularTint semantic (which controls the balance between material and light colors in specular highlighting). Providing a float value for the material property applies that value for all pixels rendered using the material; to provide variation in the semantic’s value across a surface, use a grayscale texture image instead.

## See Also

### Working with a Material Property’s Value

var stringValue: String?

The string value for the material.

var urlValue: URL?

The URL value for the material property—typically, the URL to a texture image.

var textureSamplerValue: MDLTextureSampler?

A texture sampler object that provides the texture image value for the material property.

var color: CGColor?

The color value for the material property.

var float2Value: vector_float2

The 2-component floating-point vector value for the material property.

var float3Value: vector_float3

The 3-component floating-point vector value for the material property.

var float4Value: vector_float4

The 4-component floating-point vector value for the material property.

var matrix4x4: matrix_float4x4

The 4 x 4 floating-point matrix value for the material property.

