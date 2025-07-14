

- RealityKit
- MeshResource
-  init(from:) 

Initializer

# init(from:)

Synchronously creates a mesh resource from a low-level mesh.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor @preconcurrency
convenience init(from mesh: LowLevelMesh) throws
```

## Parameters 

`mesh`  

The vertex data that defines the mesh.

## See Also

### Creating a low level resource

convenience init(from: LowLevelMesh) async throws

Asynchronously creates a mesh resource from a low-level mesh.

var lowLevelMesh: LowLevelMesh?

The low-level mesh that this mesh is built from, if any.

