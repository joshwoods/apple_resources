

- Model I/O
- MDLMaterial
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Returns the material property at the specified index in the material, for use with subscript syntax.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
subscript(idx: Int) -> MDLMaterialProperty? { get }
```

## Parameters 

`idx`  

An index in the material’s list of material properties; must be less than the value of count.

## Return Value

The material property at the specified index.

## Discussion

The ordering of material properties in a material is arbitrary, but you can use this method (together with the count property) to iterate through the material’s complete list of material properties. You can also iterate through material properties using Fast Enumeration.

## See Also

### Accessing material properties with subscript syntax

subscript(String) -> MDLMaterialProperty?

Returns the material property with the specified name, for use with subscript syntax.

var count: Int

The number of material properties in the material.

