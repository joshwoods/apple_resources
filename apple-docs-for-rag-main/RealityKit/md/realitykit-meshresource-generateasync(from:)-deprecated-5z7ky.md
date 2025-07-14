

- RealityKit
- MeshResource
-  generateAsync(from:) Deprecated

Type Method

# generateAsync(from:)

Create a mesh resource from contents asynchronously.

iOS 15.0–18.0DeprecatediPadOS 15.0–18.0DeprecatedMac Catalyst 15.0–18.0DeprecatedmacOS 12.0–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor @preconcurrency
static func generateAsync(from content: MeshResource.Contents) -> LoadRequest
```

## See Also

### Creating a mesh resource

static func generate(from: MeshResource.Contents) throws -> MeshResource

Create a mesh resource from contents.

static func generate(from: [MeshDescriptor]) throws -> MeshResource

Create a mesh resource from a list of mesh descriptors.

convenience init(from: [MeshDescriptor]) async throws

Initialize a mesh resource from descriptors asynchronously.

convenience init(from: MeshResource.Contents) async throws

Initialize a mesh resource from contents asynchronously.

convenience init(shape: ShapeResource) async

Generates a MeshResource from a ShapeResource.

convenience init(shape: ShapeResource)

Generates a MeshResource from a ShapeResource.

static func generateAsync(from: [MeshDescriptor]) -> LoadRequest&lt;MeshResource>

Create a mesh resource from a list of mesh descriptors asynchronously.

Deprecated

