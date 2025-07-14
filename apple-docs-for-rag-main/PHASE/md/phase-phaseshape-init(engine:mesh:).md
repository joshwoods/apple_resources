

- PHASE
- PHASEShape
-  init(engine:mesh:) 

Initializer

# init(engine:mesh:)

Creates an object that the given geometric data shapes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
init(
    engine: PHASEEngine,
    mesh: MDLMesh
)
```

## Parameters 

`engine`  

The object that controls this class’s associated audio output.

`mesh`  

A collection of points that connect to form a shape.

## See Also

### Creating a Shape

convenience init(engine: PHASEEngine, mesh: MDLMesh, materials: [PHASEMaterial])

Creates an object of a specific material that the given geometric data shapes.

