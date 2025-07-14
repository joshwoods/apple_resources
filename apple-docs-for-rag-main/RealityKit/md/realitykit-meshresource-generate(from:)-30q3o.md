

- RealityKit
- MeshResource
-  generate(from:) 

Type Method

# generate(from:)

Create a mesh resource from contents.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
@MainActor @preconcurrency
static func generate(from content: MeshResource.Contents) throws -> MeshResource
```

## See Also

### Creating a mesh resource

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

static func generateAsync(from: MeshResource.Contents) -> LoadRequest&lt;MeshResource>

Create a mesh resource from contents asynchronously.

Deprecated

static func generateAsync(from: [MeshDescriptor]) -> LoadRequest&lt;MeshResource>

Create a mesh resource from a list of mesh descriptors asynchronously.

Deprecated

