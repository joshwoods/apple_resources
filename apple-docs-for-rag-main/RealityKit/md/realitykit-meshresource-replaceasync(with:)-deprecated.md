

- RealityKit
- MeshResource
-  replaceAsync(with:) Deprecated

Instance Method

# replaceAsync(with:)

Replace the contents of this mesh resource asynchronously.

iOS 15.0–18.0DeprecatediPadOS 15.0–18.0DeprecatedMac Catalyst 15.0–18.0DeprecatedmacOS 12.0–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor @preconcurrency
func replaceAsync(with content: MeshResource.Contents) -> LoadRequest
```

## Discussion

Note

The contents of the modified mesh resource will not be synced between network clients.

## See Also

### Configuring the resource

var expectedMaterialCount: Int

The number of material entries required to render the mesh resource.

func replace(with: MeshResource.Contents) throws

Replace the contents of this mesh resource.

func replace(with: MeshResource.Contents) async throws

Replace the contents of this mesh resource asynchronously.

