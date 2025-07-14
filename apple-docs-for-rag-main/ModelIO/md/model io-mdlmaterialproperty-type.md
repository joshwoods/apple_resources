

- Model I/O
- MDLMaterialProperty
-  type 

Instance Property

# type

The data type stored in the material property’s value.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var type: MDLMaterialPropertyType { get set }
```

## Discussion

Each semantic value has one or more data types that are appropriate for its value. For example, the MDLMaterialSemantic.baseColor semantic provides per-pixel colors for a rendered surface, so appropriate values for that semantic include scalars (interpreted as a grayscale color), colors, texture images, or URLs that refer to texture images. The MDLMaterialSemantic.ambientOcclusionScale semantic provides a scale factor for the effect of ambient occlusion shading, so an appropriate value is a scalar or a grayscale image that varies that scalar value across the surface of the material.

## See Also

### Using a Material Property

var name: String

A descriptive name for the material property.

var semantic: MDLMaterialSemantic

The semantic meaning for the material property’s value.

