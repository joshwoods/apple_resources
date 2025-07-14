

- RealityKit
- MeshResource
-  init(from:) 

Initializer

# init(from:)

Initialize a mesh resource from descriptors asynchronously.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
nonisolated
convenience init(from descriptors: [MeshDescriptor]) async throws
```

## See Also

### Creating a mesh resource

static func generate(from: MeshResource.Contents) throws -> MeshResource

Create a mesh resource from contents.

static func generate(from: [MeshDescriptor]) throws -> MeshResource

Create a mesh resource from a list of mesh descriptors.

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

