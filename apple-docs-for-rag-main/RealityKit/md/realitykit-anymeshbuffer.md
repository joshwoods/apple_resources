

- RealityKit
-  AnyMeshBuffer 

Structure

# AnyMeshBuffer

Mesh buffer stored in the container.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct AnyMeshBuffer
```

## Topics

### Inspecting a mesh buffer

var count: Int

var elementType: MeshBuffers.ElementType

var id: MeshBuffers.Identifier

var rate: MeshBuffers.Rate

func get&lt;Value>(Value.Type) -> MeshBuffer&lt;Value>?

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

struct MeshInstanceCollection

An object that holds a collection of mesh resource instances.

struct MeshModelCollection

An object that holds a collection of mesh models.

struct MeshPartCollection

An object that holds a collection of mesh parts.

