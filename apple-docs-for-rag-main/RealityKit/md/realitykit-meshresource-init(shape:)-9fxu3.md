

- RealityKit
- MeshResource
-  init(shape:) 

Initializer

# init(shape:)

Generates a MeshResource from a ShapeResource.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
convenience init(shape resource: ShapeResource) async
```

## Parameters 

`resource`  

The ShapeResource which will be used for generating the mesh.

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

convenience init(shape: ShapeResource)

Generates a MeshResource from a ShapeResource.

static func generateAsync(from: MeshResource.Contents) -> LoadRequest&lt;MeshResource>

Create a mesh resource from contents asynchronously.

Deprecated

static func generateAsync(from: [MeshDescriptor]) -> LoadRequest&lt;MeshResource>

Create a mesh resource from a list of mesh descriptors asynchronously.

Deprecated

