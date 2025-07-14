

- Model I/O
- MDLMaterial
-  removeAllProperties() 

Instance Method

# removeAllProperties()

Removes all material properties from the material.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func removeAllProperties()
```

## See Also

### Working with individual material properties

func propertyNamed(String) -> MDLMaterialProperty?

Returns the material property with the specified name.

func property(with: MDLMaterialSemantic) -> MDLMaterialProperty?

Returns the material property for the specified material semantic.

func properties(with: MDLMaterialSemantic) -> [MDLMaterialProperty]

Returns the complete list of material properties that match the specified material semantic.

func setProperty(MDLMaterialProperty)

Adds a new material property to or replaces an existing material property in the material.

func remove(MDLMaterialProperty)

Removes the specified material property from the material.

