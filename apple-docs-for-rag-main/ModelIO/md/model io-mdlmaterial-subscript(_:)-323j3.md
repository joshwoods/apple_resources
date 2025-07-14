

- Model I/O
- MDLMaterial
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Returns the material property with the specified name, for use with subscript syntax.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
subscript(name: String) -> MDLMaterialProperty? { get }
```

## Parameters 

`name`  

The name value of a material property in the material.

## Return Value

The material property with the specified name, or `nil` if the material does not contain a material property with that name.

## Discussion

This method is equivalent to the propertyNamed(_:) method but allows for the use of subscript syntax for reading material properties. To write material properties to the material, use the setProperty(_:) method.

## See Also

### Accessing material properties with subscript syntax

subscript(Int) -> MDLMaterialProperty?

Returns the material property at the specified index in the material, for use with subscript syntax.

var count: Int

The number of material properties in the material.

