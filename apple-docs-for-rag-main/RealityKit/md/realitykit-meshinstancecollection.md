

- RealityKit
-  MeshInstanceCollection 

Structure

# MeshInstanceCollection

An object that holds a collection of mesh resource instances.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct MeshInstanceCollection
```

## Topics

### Creating a collection

init()

init([MeshResource.Instance])

### Using the collection

var count: Int

Number of instances.

var isEmpty: Bool

True if there are no instances.

func insert(MeshResource.Instance) -> Bool

Add a new instance to the container. Returns true if added.

func remove(id: String) -> MeshResource.Instance?

Remove an instance by name.

func removeAll()

Remove all the instances.

func update(MeshResource.Instance) -> MeshResource.Instance?

Update an existing instance. The old instance is returned.

subscript(String) -> MeshResource.Instance?

Read an instance given its name.

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

struct MeshModelCollection

An object that holds a collection of mesh models.

struct MeshPartCollection

An object that holds a collection of mesh parts.

