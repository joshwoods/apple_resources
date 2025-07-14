

- Model I/O
- MDLMaterial
-  properties(with:) 

Instance Method

# properties(with:)

Returns the complete list of material properties that match the specified material semantic.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func properties(with semantic: MDLMaterialSemantic) -> [MDLMaterialProperty]
```

## Parameters 

`semantic`  

The semantic value of a material property in the material.

## Return Value

The material properties for the specified semantic, or an empty array if the material does not contain a material property for that semantic.

## Discussion

Material semantics identify the intended use of a material property in shading. Some semantic values, such as MDLMaterialSemantic.specular, are part of the material’s scatteringFunction property that determines its response to lighting. Another semantic value, such as MDLMaterialSemantic.opacity, determine the opacity of material rendering.

## See Also

### Working with individual material properties

func propertyNamed(String) -> MDLMaterialProperty?

Returns the material property with the specified name.

func property(with: MDLMaterialSemantic) -> MDLMaterialProperty?

Returns the material property for the specified material semantic.

func setProperty(MDLMaterialProperty)

Adds a new material property to or replaces an existing material property in the material.

func remove(MDLMaterialProperty)

Removes the specified material property from the material.

func removeAllProperties()

Removes all material properties from the material.

