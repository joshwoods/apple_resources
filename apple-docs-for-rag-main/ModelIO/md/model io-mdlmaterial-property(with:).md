

- Model I/O
- MDLMaterial
-  property(with:) 

Instance Method

# property(with:)

Returns the material property for the specified material semantic.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func property(with semantic: MDLMaterialSemantic) -> MDLMaterialProperty?
```

## Parameters 

`semantic`  

The semantic value of a material property in the material.

## Return Value

The material property for the specified semantic, or `nil` if the material does not contain a material property for that semantic.

## Discussion

Material semantics identify the intended use of a material property in shading. Some semantic values, such as MDLMaterialSemantic.specular, are part of the material’s scatteringFunction property that determines its response to lighting; others, such as MDLMaterialSemantic.opacity, determine other aspects of material rendering.

## See Also

### Working with individual material properties

func propertyNamed(String) -> MDLMaterialProperty?

Returns the material property with the specified name.

func properties(with: MDLMaterialSemantic) -> [MDLMaterialProperty]

Returns the complete list of material properties that match the specified material semantic.

func setProperty(MDLMaterialProperty)

Adds a new material property to or replaces an existing material property in the material.

func remove(MDLMaterialProperty)

Removes the specified material property from the material.

func removeAllProperties()

Removes all material properties from the material.

