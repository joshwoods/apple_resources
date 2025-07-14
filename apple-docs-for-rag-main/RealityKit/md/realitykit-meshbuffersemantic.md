

- RealityKit
-  MeshBufferSemantic 

Protocol

# MeshBufferSemantic

A protocol that holds an identifier value for mesh buffers.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
protocol MeshBufferSemantic : Identifiable
```

## Topics

### Associated Types

associatedtype Element

**Required**

### Instance Properties

var id: MeshBuffers.Identifier

**Required**

## Relationships

### Inherits From

- Identifiable

### Conforming Types

- MeshBuffers.Semantic

## See Also

### Mesh description

struct MeshBuffer

Mesh buffer containing elements of any type.

protocol MeshBufferContainer

Conforming objects contain a table of mesh buffers.

enum MeshBuffers

An object that holds the data for an model entity’s mesh.

struct AnyMeshBuffer

Mesh buffer stored in the container.

struct MeshInstanceCollection

An object that holds a collection of mesh resource instances.

struct MeshModelCollection

An object that holds a collection of mesh models.

struct MeshPartCollection

An object that holds a collection of mesh parts.

