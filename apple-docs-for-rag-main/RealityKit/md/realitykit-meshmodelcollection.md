

- RealityKit
-  MeshModelCollection 

Structure

# MeshModelCollection

An object that holds a collection of mesh models.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct MeshModelCollection
```

## Topics

### Creating a collection

init()

init([MeshResource.Model])

### Using the collection

var count: Int

Number of models.

var isEmpty: Bool

True if there are no models.

func insert(MeshResource.Model) -> Bool

Add a new model to the container. Returns true if added.

func remove(id: String) -> MeshResource.Model?

Remove a model by id.

func removeAll()

Remove all the models.

func update(MeshResource.Model) -> MeshResource.Model?

Update an existing model. The old model is returned.

subscript(String) -> MeshResource.Model?

Read a model given its id.

### Default Implementations

Collection Implementations

ExpressibleByArrayLiteral Implementations

Sequence Implementations

## Relationships

### Conforms To

- Collection
- Copyable
- ExpressibleByArrayLiteral
- Sequence

## See Also

### Mesh description

struct MeshBuffer

Mesh buffer containing elements of any type.

protocol MeshBufferContainer

Conforming objects contain a table of mesh buffers.

protocol MeshBufferSemantic

A protocol that holds an identifier value for mesh buffers.

enum MeshBuffers

An object that holds the data for an model entity’s mesh.

struct AnyMeshBuffer

Mesh buffer stored in the container.

struct MeshInstanceCollection

An object that holds a collection of mesh resource instances.

struct MeshPartCollection

An object that holds a collection of mesh parts.

