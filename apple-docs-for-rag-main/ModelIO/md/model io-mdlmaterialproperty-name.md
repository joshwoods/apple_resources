

- Model I/O
- MDLMaterialProperty
-  name 

Instance Property

# name

A descriptive name for the material property.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var name: String { get set }
```

## Discussion

A material property’s name is not used for rendering, but it can be useful in debugging. Model Model I/O may set a material property’s name to a format-specific value when loading materials from an MDLAsset object.

## See Also

### Using a Material Property

var semantic: MDLMaterialSemantic

The semantic meaning for the material property’s value.

var type: MDLMaterialPropertyType

The data type stored in the material property’s value.

