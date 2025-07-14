

- RealityKit
- MeshResource
-  replace(with:) 

Instance Method

# replace(with:)

Replace the contents of this mesh resource.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
@MainActor @preconcurrency
func replace(with content: MeshResource.Contents) throws
```

## Discussion

Note

The contents of the modified mesh resource will not be synced between network clients.

## See Also

### Configuring the resource

var expectedMaterialCount: Int

The number of material entries required to render the mesh resource.

func replace(with: MeshResource.Contents) async throws

Replace the contents of this mesh resource asynchronously.

func replaceAsync(with: MeshResource.Contents) -> LoadRequest&lt;MeshResource>

Replace the contents of this mesh resource asynchronously.

Deprecated

