

- Model I/O
- MDLMaterial
-  propertyNamed(\_:) 

Instance Method

# propertyNamed(\_:)

Returns the material property with the specified name.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func propertyNamed(_ name: String) -> MDLMaterialProperty?
```

## Parameters 

`name`  

The name value of a material property in the material.

## Return Value

The material property with the specified name, or `nil` if the material does not contain a material property with that name.

## Discussion

Material property names are not related to their use in rendering. Instead, you can assign descriptive names to material properties and use this method to keep track of them.

## See Also

### Working with individual material properties

func property(with: MDLMaterialSemantic) -> MDLMaterialProperty?

Returns the material property for the specified material semantic.

func properties(with: MDLMaterialSemantic) -> [MDLMaterialProperty]

Returns the complete list of material properties that match the specified material semantic.

func setProperty(MDLMaterialProperty)

Adds a new material property to or replaces an existing material property in the material.

func remove(MDLMaterialProperty)

Removes the specified material property from the material.

func removeAllProperties()

Removes all material properties from the material.

