

- RealityKit
- MeshResource
-  init(from:) 

Initializer

# init(from:)

Creates a MeshResource from the provided MeshAnchor.

visionOS 2.0+

``` source
@MainActor @preconcurrency
convenience init(from meshAnchor: MeshAnchor) async throws
```

## Parameters 

`meshAnchor`  

A MeshAnchor that will be used to generate the MeshResource.

## See Also

### Creating a mesh from an anchor

convenience init(from: PlaneAnchor) async throws

