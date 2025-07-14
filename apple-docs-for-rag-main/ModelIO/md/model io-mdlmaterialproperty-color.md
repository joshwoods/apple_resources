

- Model I/O
- MDLMaterialProperty
-  color 

Instance Property

# color

The color value for the material property.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var color: CGColor? { get set }
```

## Discussion

A material property with a color value uses a uniform color for all pixels rendered using the material. This option is useful for base colors of solid-color objects, and also for material semantics where variation across the surface of the material is unnecessary. To vary colors across a surface, use a texture image instead.

## See Also

### Working with a Material Property’s Value

var stringValue: String?

The string value for the material.

var urlValue: URL?

The URL value for the material property—typically, the URL to a texture image.

var textureSamplerValue: MDLTextureSampler?

A texture sampler object that provides the texture image value for the material property.

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

