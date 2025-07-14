

- RealityKit
- SimpleMaterial
-  init(color:roughness:isMetallic:) 

Initializer

# init(color:roughness:isMetallic:)

Creates a simple material with specific characteristics in macOS.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+

``` source
init(
    color: SimpleMaterial.Color,
    roughness: MaterialScalarParameter = 0.0,
    isMetallic: Bool
)
```

## Parameters 

`color`  

The color of the material.

`roughness`  

The roughness of the material.

`isMetallic`  

A Boolean indicating whether the material should have a metallic appearance.

## See Also

### Creating a simple material

init()

Creates a simple material.

init(color: SimpleMaterial.Color, roughness: MaterialScalarParameter, isMetallic: Bool)

Creates a simple material with specific characteristics in macOS.

