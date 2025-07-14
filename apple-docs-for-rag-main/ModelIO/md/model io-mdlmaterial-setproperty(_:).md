

- Model I/O
- MDLMaterial
-  setProperty(\_:) 

Instance Method

# setProperty(\_:)

Adds a new material property to or replaces an existing material property in the material.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func setProperty(_ property: MDLMaterialProperty)
```

## Parameters 

`property`  

The material property object to add to the material.

## Discussion

If the material already contains a material property with the same name or semantic, this method replaces that material property. Otherwise, this method adds the specified material property to the material.

## See Also

### Working with individual material properties

func propertyNamed(String) -> MDLMaterialProperty?

Returns the material property with the specified name.

func property(with: MDLMaterialSemantic) -> MDLMaterialProperty?

Returns the material property for the specified material semantic.

func properties(with: MDLMaterialSemantic) -> [MDLMaterialProperty]

Returns the complete list of material properties that match the specified material semantic.

func remove(MDLMaterialProperty)

Removes the specified material property from the material.

func removeAllProperties()

Removes all material properties from the material.

