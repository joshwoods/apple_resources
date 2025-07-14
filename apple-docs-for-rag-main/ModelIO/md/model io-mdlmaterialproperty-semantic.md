

- Model I/O
- MDLMaterialProperty
-  semantic 

Instance Property

# semantic

The semantic meaning for the material property’s value.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var semantic: MDLMaterialSemantic { get set }
```

## Discussion

A material semantic determines how the material property’s value should be interpreted to produce a specific surface appearance in rendering. For example, the MDLMaterialSemantic.baseColor semantic defines the default color of each pixel on a rendered surface before shading effects are applied.

When Model I/O loads materials from an MDLAsset object, it automatically selects the appropriate standard semantics for the surface rendering descriptions in the asset file.

## See Also

### Using a Material Property

var name: String

A descriptive name for the material property.

var type: MDLMaterialPropertyType

The data type stored in the material property’s value.

