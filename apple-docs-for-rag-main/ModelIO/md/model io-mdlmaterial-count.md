

- Model I/O
- MDLMaterial
-  count 

Instance Property

# count

The number of material properties in the material.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var count: Int { get }
```

## See Also

### Accessing material properties with subscript syntax

subscript(String) -> MDLMaterialProperty?

Returns the material property with the specified name, for use with subscript syntax.

subscript(Int) -> MDLMaterialProperty?

Returns the material property at the specified index in the material, for use with subscript syntax.

