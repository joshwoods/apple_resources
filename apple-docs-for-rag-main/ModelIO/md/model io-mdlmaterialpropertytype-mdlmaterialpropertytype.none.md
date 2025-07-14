

- Model I/O
- MDLMaterialPropertyType
-  MDLMaterialPropertyType.none 

Case

# MDLMaterialPropertyType.none

The material property’s value has not been initialized.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
case none
```

## Discussion

Set one of the properties listed in Working with a Material Property’s Value to provide a value for the material property. After setting a value, the type property reflects the data type of that value.

## See Also

### Constants

case string

The material’s value is a string.

case URL

The material property’s value is a URL—typically, a URL referencing a texture image.

case texture

The material property’s value is a MDLTextureSampler object that provides both a texture image and texture rendering parameters.

case color

The material property’s value is a uniform color.

case float

The material property’s value is a floating-point scalar.

case float2

The material property’s value is a 2-component floating-point vector.

case float3

The material property’s value is a 3-component floating-point vector.

case float4

The material property’s value is a 4-component floating-point vector.

case matrix44

The material property’s value is a 4 x 4 floating-point matrix.

