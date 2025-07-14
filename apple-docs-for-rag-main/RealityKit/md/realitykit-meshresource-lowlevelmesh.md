

- RealityKit
- MeshResource
-  lowLevelMesh 

Instance Property

# lowLevelMesh

The low-level mesh that this mesh is built from, if any.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor @preconcurrency
var lowLevelMesh: LowLevelMesh? { get }
```

## Discussion

If this mesh is not built from a LowLevelMesh, it returns nil.

## See Also

### Creating a low level resource

convenience init(from: LowLevelMesh) async throws

Asynchronously creates a mesh resource from a low-level mesh.

convenience init(from: LowLevelMesh) throws

Synchronously creates a mesh resource from a low-level mesh.

