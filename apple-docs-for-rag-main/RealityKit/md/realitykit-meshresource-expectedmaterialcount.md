

- RealityKit
- MeshResource
-  expectedMaterialCount 

Instance Property

# expectedMaterialCount

The number of material entries required to render the mesh resource.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
var expectedMaterialCount: Int { get }
```

## See Also

### Configuring the resource

func replace(with: MeshResource.Contents) throws

Replace the contents of this mesh resource.

func replace(with: MeshResource.Contents) async throws

Replace the contents of this mesh resource asynchronously.

func replaceAsync(with: MeshResource.Contents) -> LoadRequest&lt;MeshResource>

Replace the contents of this mesh resource asynchronously.

Deprecated

